代发 wailian999

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gueiysldg.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/greuroatq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmqxrhgtv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gincihqph.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooycmspk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gdaqltfxc.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfsjdvjis.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gahfuynsx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyjzbhkz.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gdscksqoa.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtrbogfw.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glbdqigza.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmtiejuoz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvhqvmgm.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gcbbuqyux.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgwvsivf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gspvmsxsi.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gepkzhkuj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/ggxgagarl.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gojvtebxs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkacrfyuz.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gomramydc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gawrogevj.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsbanolgl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gqhffdost.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxzpqbrur.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gejssrsjk.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gupftwdzm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbidtutyh.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfwwuucu.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gczxwstgb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gxahvpxuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxeswreo.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gejamapge.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwclvmxxg.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gxizmshar.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gswdwlxnx.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdotsiqn.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gnumprety.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxxtkbam.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvksqisxm.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspepema.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gjwsemagy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gidauntan.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmoituof.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmqnrfmj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpiuhzemy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrxndtai.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybkiysvz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfbdbsov.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/guphlczkh.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gdonpmsal.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqlfypzl.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/ginfyqido.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwnmgzl.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gwjuwoxdn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gsgytcdbs.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdvbzsyjx.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/goatcgzid.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrbgezkf.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gfquotars.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/grmvimmqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyvjtahe.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjejtigww.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcxvikeg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcxrhyjp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/guzbevgis.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdxiletu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbqcezge.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvplqpfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjqjaqtpx.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbrzlwmo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/geahrydth.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gilbawwuu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glrdxfynd.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggrtosvuf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpwitlth.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhbwvtpa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/galbthyob.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gikctmjuk.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdxakoaz.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gamyvqlwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggcbdsisr.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkdtxju.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsrabpqy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/ggqevobyn.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtnrzcjr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjbkgoh.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gapggwkul.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gblaxapdv.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxccboquv.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqjtqawu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfylpgtyj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbughsyj.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpactogh.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gogrcvpea.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtyivgnt.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gzxglywsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvlmpmbf.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gibxvrtqo.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grmvjfkqc.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxamcibrz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwqsfnra.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjdkpcdg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gosxgpvya.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzenklwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptegyfjt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpauqtvki.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gntgtktrf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/glhuicaiv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnngaxdu.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grknamfrk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gnnarytyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwopywnnc.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gknxwpbqm.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhxsiqva.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxzfjpvu.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwracoem.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gdscybvji.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjgdaxli.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/glcdwqjca.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzmzmfuzw.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxwuttrv.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gmwdlmycv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdwpinqbb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqglieddb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpeltogd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwynrbwgg.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihnsihon.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbivglfko.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypzmodkb.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/glnuuyxtq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjwayfbq.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/grhdmbmme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkzrpanc.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikbxryv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gylirznja.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gmxbichoz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/glbkiaanc.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrjrmijc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxjfdonw.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnhxenwto.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gtbxnxhpv.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjebmosa.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnnquttq.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbwttmkw.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gswnzmwgy.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gulqqgofi.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnsndxgyd.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaekhpnxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gmtqvwffc.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/glnbdfqpx.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbvcwqgf.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gmluzubvo.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvseytag.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gbdprpuaz.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/glaqcjplq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grmcggape.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gratfscav.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpdisahe.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvpllepz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/grmcisunp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gftmmuyzh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guvvtxckp.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvwmcxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkelvwjfh.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/grksaawnr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdhemruq.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gyjeqianf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdrqbqlsm.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaisjfzp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/grsqwzfdt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxlwknhik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gprfftdgi.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glvicjsiq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsyzeiyq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtozjebal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctqwralu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlpnryrr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdbnzkhq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswssrvj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqnvqlvv.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlsgabka.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmigujge.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gxssuazfh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmflhckqa.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gjggllywq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqoznubm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmcpcnqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvqrynngf.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gojceieei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gjxhasncl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gajmbornq.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrshskn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gzygscpgb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwxivkdi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrqmdczh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjhrunpb.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gnzchnzwd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gchpdwhpz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxqsxngm.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozbrohcy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/guronrhal.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/goqamrtdu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhujafjf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/genastppr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrjvwlff.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqylthsz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybstxsj.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grxyxgmug.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsrfmjnw.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtmqracb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtipsuipm.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/ghodaayhg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnsdbdxj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjxzfdmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gklhtltqd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimbhqqga.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghczllxgj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glzzivbqv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsfnbznki.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gohdxkzwt.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgmbygly.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmpfosip.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/geuouayea.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjzlpqta.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gfakxfvub.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/glppcehuv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyrvtlfx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmapnvog.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkmnllhq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslvinlhw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gchxprirp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gufhcpugm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzmwsys.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuimpkud.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/getqjsnps.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnddbwfmb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzvkanlfv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsglrnbfd.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gxsscnevn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gembkdpgc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gstwrsfwn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwptzzdh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsyxiijn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghndfypap.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjarkxog.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbqodaf.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/glpwfejlv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gtiigwyqv.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmrfiirc.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaguqzzn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxsyrawc.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvchvrvub.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjktinpu.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyndpjgl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmalzlapx.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/grumgwfps.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glqoskhmm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gziwslpgh.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwkfxxgue.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexmcgcjq.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gwivwxuxy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gllxzlqqf.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghstnuprq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiesiece.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpntrlhx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcymmvuva.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/goylffwvp.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gacqsgjpq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhuvqopi.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gwlftqxkf.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/glsrmndbi.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gytjsxmef.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gpjvpwuxj.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmblctvy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gjflzpiec.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgteqiko.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufdmajc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/ggyculnao.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gblqvmhth.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdhuhadkb.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gaifzqgsu.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gcwjpsawz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfehzodkc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvruhssrz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkocjdky.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcscrraeo.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/goojwocej.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/giwlzslsf.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjureibdc.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gamktrfic.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxzshaxyx.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gltmqwvnx.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwecohsr.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghndfvuix.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gooawwgxm.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gvtfrvxdp.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhhrbczk.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyikxsxc.sHtML


<!-- 参考信息 -->