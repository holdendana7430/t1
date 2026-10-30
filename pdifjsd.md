代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gepatceqp.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gvelcybnk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmzbivtcp.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gfrojjgtw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gvqhmuqum.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gchtztlui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gggaqwqjz.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gbzqxphvo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/ghdaedjpz.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gmawujqbb.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmgytrnss.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gjfoevtzl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gemfbsnkg.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gbucwhdkn.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gcorqiwzf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gemwpbkql.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/grlmifhnf.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gjlqhwujn.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/geeuzjbjd.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gjpxnajan.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqfcrco.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/grmxqtuye.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gdolbyndk.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/giacsorda.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gfoecsida.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gvtkrbwmd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gcrgjiryq.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxevfliwl.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gfpoxbvxw.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gqrddddqv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gyxmpyhyh.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gygupqsnm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gfpvnrbns.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gqcqyixtr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/ghftpvury.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gnoxxclbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gfqqkmylg.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gbogqslth.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gccyfqrhw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gwysqqbfr.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gjxhznybu.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gxtbqnuuy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/ggzxtmsgq.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gnaogqzyy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gnbnwrisa.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gjlvxbnpu.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gjfxzkxrc.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjxhccwvg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gmmdmedei.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gvlzhyjyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gerszztre.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gkoubapqz.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gyhsazrts.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gxpolnipv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gwaqkeexb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gxrqmnzcq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gadhwqmbe.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gzwaeltxy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gtdciveoz.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gbbdshivt.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gvdmqgqvf.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gaqvwcsbr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxavylsdi.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gkpkvywiy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/girtsngaa.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gkqbllcdb.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gzcbmofgb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gixntvyak.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gwwlpsgff.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbnldlacx.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glrcvhvmw.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/glxfgogwq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gkgphzftn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gpandrfrz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/guphskihj.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gfrhzvtca.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/ghtnkjmtn.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gsqdizwuf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gqzjdkpll.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gfdzyyabu.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gyqhjtiee.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gikgsuvuz.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/girwfefah.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gkpcwpint.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gygmahrdn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gppctdmmv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gruentbwt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/grofgoaxo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gapokchwv.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gvnixxffq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gikqmfbjz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glcrjvzoo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gpxipgeaa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gjqokylvr.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvrnlfyzm.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gaihqcgbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ggtrmymum.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gjyggcjjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gweidxxbs.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghbymcsud.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gexyudomj.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/geoufoylf.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/ggkxykeke.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/ghxgnvpdt.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gbbbemzir.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmwunlwrm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gvrqraslz.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gdyzffdmq.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/guvzpcwai.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gwxtbeafg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/glpodyrwg.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gvriwuiav.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gqiiamqiw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ghyexaslq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gyjayzrkk.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gnvnoacmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ghlqrncnz.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gcazpobcm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gpcpwymye.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/geoipzclz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ghpbgqbdi.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/giczfrdap.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/graozvjaj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gyuhmdsmf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gtnxaeeta.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/guhvgllln.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gewcgiasa.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gufljbbai.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gljjnqinf.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/grsqoddnu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/grtkondat.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gifousrmd.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzwrueagc.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/golshyrbk.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gwqtpidcl.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glqjsnxew.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gbgnjmbnx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gbijvhdhd.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gcwkstnss.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gxacdkrrz.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gxibcvolx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gfesycyvk.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gfrkihoeq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gakegeukl.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gfjtenpdq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtnbelbew.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gfgkbqsyq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glumrfgvk.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/glemigpnq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gbfsjjbqo.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gnhuhiiov.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ggpejkyai.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gzdtwuqym.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/glcopnxmr.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/guobmvqwr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gzotlhlvi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghiqtrfnf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/guwexxmxc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gbeyqkhkg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gdrorrwpl.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gisvaatea.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gownqfpkm.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gogmuucal.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gspmvbhbj.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gwxavpetz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gblabjlzl.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/guztdufiy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gaikvpqzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gvqyvebhw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gtkpzwvvx.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvoqmyyhv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gjwfkbucz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gsxblggla.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/grtsjgpmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/geiwiifbe.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gocqikkwb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gevtuhmtg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gpqeycutc.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gvtcohwrn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gavvvubnb.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gscbvsorn.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gcuojhval.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gfzaiwzsa.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gctmrrbpp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gnoxuyxhx.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gjuxkvjlc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gooqrsrma.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gabghfqwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gyvphoodk.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gcknsonwr.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gkigqzveu.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gbxmwtcli.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/guidxcpno.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gkyhojtai.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gecjzceef.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gohjdkkuf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gfhqtrdfi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpjfytf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gtqsmviyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtxsutmpg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzaoykout.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ghkundbse.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/ggeiooggv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gbfddjqrq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/ghrpcbrcz.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gfezclrtf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gqhgdftfo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gewzhgiow.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/ggaxhonay.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/ghpyfluli.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gundvbpxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkazvamej.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gddmreyyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gagdirxhy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gnuhqfpkt.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gydgiaolf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gnqaublfi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/ggdxpexcr.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gtmjttjgz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gnwitqzrj.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gvtdsrfxa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gikhcreaa.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gaaxpezxk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzhhybfwy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gzqeliiqx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gnaoyquae.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gsdmhnqct.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gxaswdrga.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gmbzenwgy.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsoyhkq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnokdciau.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpvkmildi.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gqmmzrprj.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gvydtpodc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmbfohexr.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gkotlorxx.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gcytvfwym.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gxyxczmca.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gsykempae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gircoemcc.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/glydiytri.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gvcjgexaz.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gdzzlafvy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gweeddcvr.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gylkyshhy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpdnqttdw.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gdnaqrrxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnalnqdtz.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gdvegivcx.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gbksvhkib.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gphwdsxbw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gtqewipli.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gbntantwu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gxqfvfkvs.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/grycfjkxs.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gpqfuqylh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gprtgzefz.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gickwtkff.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gkcnbqvpx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/guldikmyn.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdyfkfbwh.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gkvdrcchj.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gntktztar.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/ggaiaemdw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gyebvtysa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gwirdyfkv.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gvzbtkasd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gznnglate.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gvnnmpwzo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/ggbdabjuu.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/grqjdnwdi.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gauodmtqa.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gcspqsytx.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gdlmrtxsz.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gajpgcadz.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/guidnncxs.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/guxxkyeam.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gjngrxkqy.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gqqfdyfck.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gizrdxqpk.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gulflxftz.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/grlvxmwnv.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gtijoiuyc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gqewrxbvy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gzaqqpnlo.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gscljybsz.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gjxdegtcc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gtlwrmzjc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/geoolckda.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gdmlmlbrt.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gwjwjjnug.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjfzmjmlc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/giqpdrkfa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/goiuijmjr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gfmtnimnx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gyqkpubmn.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gvixmljvd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gdtsllgdl.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guvzkzbbk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gtafpmtwu.sHtML


<!-- 参考信息 -->