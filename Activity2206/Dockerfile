FROM mcr.microsoft.com/dotnet/aspnet:6.0
ADD wget https://github.com/nopSolutions/nopCommerce/releases/download/release-4.50.3/nopCommerce_4.50.3_NoSource_linux_x64.zip /NOP/nopCommerce_4.50.3_NoSource_linux_x64.zip
RUN apt update -y && apt install unzip -y && mkdir /NOP/bin && mkdir /NOP/logs unzip nopCommerce_4.50.3_NoSource_linux_x64.zip
WORKDIR /NOP
EXPOSE 80
CMD ["/usr/bin/dotnet", "/NOP/NOP.web.dll"]