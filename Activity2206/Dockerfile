FROM mcr.microsoft.com/dotnet/sdk:6.0
ADD https://github.com/nopSolutions/nopCommerce/releases/download/release-4.50.3/nopCommerce_4.50.3_NoSource_linux_x64.zip /Nop/nopCommerce_4.50.3_NoSource_linux_x64.zip
RUN apt update && apt install unzip -y && mkdir /Nop/bin && mkdir /Nop/logs
EXPOSE 80
CMD ["/usr/bin/dotnet", "/Nop.web.dll"]