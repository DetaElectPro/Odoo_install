# Odoo install
شرح التثبيت علي نظام اوبنتو لينكس

## الخطوة الـ1
```
    sudo apt-get update
    sudo apt-get -y upgrade
    sudo apt-get install python3-pip
```
### الخطوة الـ2
 تثبيت الاعتمادات الخاصة بـ
  pip3
```
pip3 install Babel decorator docutils ebaysdk feedparser gevent greenlet html2text Jinja2 lxml Mako MarkupSafe mock num2words ofxparse passlib Pillow psutil psycogreen psycopg2 pydot pyparsing PyPDF2 pyserial python-dateutil python-openid pytz pyusb PyYAML qrcode reportlab requests six suds-jurko vatnumber vobject Werkzeug XlsxWriter xlwt xlrd
```
#### الخطوة الـ3
*يفضل استخدام 
nvm node js
```
sudo apt-get install -y npm

sudo ln -s /usr/bin/nodejs /usr/bin/node

sudo npm install -g less less-plugin-clean-css

sudo apt-get install node-less
```