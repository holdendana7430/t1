代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gtrxzvgyb.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gfroutuyo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghsnjjldv.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gswzauaca.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gjhfcnfvq.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gvvtgnpdz.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gbczyqvza.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gdgjachox.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ghakkxxbt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxgggheif.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gzivprqsj.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ghsiskrvg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gbstgamuu.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gkjjjexzu.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gtwmobdpq.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/ghxxfautv.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gvuvvduwt.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gggisaoxb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/golukrmnn.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gujpaoqmk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gyrqmxhgk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glegrhfnu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gckpmcwbk.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/glshgocqk.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gxdxzhthu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ggmlayyzr.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gpjbqoskh.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gyjcpcffk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gselfokwj.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gfheseknr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gqhilonjt.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gwcrhkpps.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gllinjdgu.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gfjrqrxfi.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gtclxerkv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gbvvistlf.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/ghqanuoag.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gnmolnlet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnwoapogz.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gkvqtxbcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gsfzferws.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gaejxannx.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gzhzortvs.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmenkwqow.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gcewbcqkj.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gmivwcevy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfyiaxjka.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gvoidzpxs.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/geovzodzw.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gsvvjaoez.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gphrhecab.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gnzmlqzlt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gznvvqkll.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gulscgpum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gxjmfwkod.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gueminfay.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/grozqczgr.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/glrowjtmy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gnszkedxo.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gwslhvtdt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmzkvljdj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gziycudfp.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/grvjabpni.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvznupqpe.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/ggsjomkkh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gncrbleli.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkaexwjiu.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gqxruzflt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gpvjbyygg.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gvtdvrjpm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gaxadhlfo.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gqeecrbiy.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gbcucoydr.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gyosjeywt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gpdlhyagz.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/geoillydy.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gwsdfzxun.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gaycgwttb.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gsnwibbnl.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gtwpkgddl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gtxameakx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gfcvzbjin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/ggaxhlrvo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/grgihknsd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/ghxujvcmb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gycoogeiw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gobniamuw.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtmndhvkd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gdvooxufy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gmkvhwiqx.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gecrqbvhb.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gveuuifoq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gblegzbcg.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/glozwmash.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gnoipwfxh.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gumollrnb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gwzhxsbyw.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gkjqqkagt.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/geqhuvtxo.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gxcdyesvf.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gvsokmxtk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gqxvmpghu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gwrkwvvay.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gpragyjvg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gvioixhhi.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gsfomakrv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gklcrzjtx.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ggdlwmtyg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gemvuwkgw.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gdcxpfwtw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gjfmhzqsk.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/goddkfzyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gzvqjlkyc.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gxaeqetjf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gftesdqjs.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gkpyduunm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gfonrogkr.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gqcwecapn.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gmilcbduf.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gpounbpxh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gjfzrhsfx.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gnmisgpwl.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gmllymomp.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/ggjbzxdeb.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gdmivdazr.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/glesogmjr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gzclwncjc.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gxjcwhdkd.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gkcbhkpqf.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gmewkktsa.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gckjtorpg.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqcnlwfmt.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gbabkbysn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/ginbhhqba.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gugxxhwjo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/geispjmlv.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gkijpsylr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gzveqikpt.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gnwwvpnix.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gqsytazmv.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gzgkorbyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glgbxbphw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/guxqipupq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbszobnoa.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gbgrlxqeo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gmreignsq.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gdlyrfipx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggsqmpgbs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/glpqmknzj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gokixqqra.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gmycyjdzd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/guyrtzbps.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/giiahyfsz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gyvxaymlq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gdysueane.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gqopvjfwd.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gqbgxdlhg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ghkibqlgf.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/ghqaeibef.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gzkdfimek.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gdgbgtuae.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpsdxxrju.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gcpdhaxlk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gnooshbek.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gydocgjxq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gygqomxzo.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjrlteuav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gehiovtzc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gdvhjcuuo.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gecbmqhpo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/grijnooyv.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gwmpouhfm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghwrtixvg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gvttqphua.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/ghmnfdodl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gbgimjljx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gejjquzyh.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gwbwhnscp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gljlmyyog.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gchlecmxm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gjzjnmauf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gbgcuwykv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/guagpztvy.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gexwuvoby.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gjkvksgyb.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/giygplwje.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gkoxurefo.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/ggbdhjnid.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gsupjesbt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gppdcjrgu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gwdmolure.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gnfxoxikc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gbeonkubk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtrzxmmpx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gtrolpbqc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gizmegqsu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gsbpleksu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/giqnqsucz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gfsocenej.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gbutuihds.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/glgkuwzdq.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gmakjfmud.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gemqvrdpf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gtuefkjii.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gxqamjyxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gmypkuvjj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gkivdazwy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/grnyqeuzl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gybzvierw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gqifgyxis.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gmkxrvvdq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gszvrzvfz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/ggvczqtun.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gunnkkhwl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gsfcmuqwx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gtcfbzmqf.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gkpaqfwcm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gocqdilan.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gxwiixrxh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjaqjvsnl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gxducyuae.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gbphvnzzb.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/ggjrpjwyu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gppfwdyxn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/giafibnpk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gwwaaqfug.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gxnxaswjc.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gczcsjnuk.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gfkveluun.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/geaxxtnrd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gvseeuzcn.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/goziktphn.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gekzpiqaz.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gmzvudijr.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gbuqlxmzk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gjaitqyan.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ghpsnfdkn.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gedinyktw.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gwwftbobx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gknefnknk.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gptptlkgj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gbmvjjgec.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/glaqreewi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gnveijoyt.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gzxlovmqm.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/glrzliveq.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gosbfnyxo.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/giyirlkpe.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gqytlhjrf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gyzdecdug.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gkrexatot.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gxlufnaxu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gkrqialmh.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gxnyjivvv.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gvqwjqade.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gucindjxq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzamomyru.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gfyihjigt.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/ggiivxxdb.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/ggrupncqz.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/guivmdqhg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/ghgolvrsg.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gaqanxwna.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gvjssfsfm.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gzuahowqz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gkvrtxeih.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gdwdwipcz.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gwlahzsur.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/grxfczlya.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gljlfgkem.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gkgejnzxw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gggtxdrsa.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gfnraxqfs.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmmfphx.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjepxas.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gomyseeet.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/goupsmkhi.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gxybyfaas.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gizjukeku.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gnbhqpxjd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gidjcxoci.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gznofesff.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gdogydhvq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/genesquoy.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gfarovgcm.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gdikmwauo.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/goxcrkbwt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmtyflegy.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gtzwztuaz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/grcztozit.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gnexphtdz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gbpqjujhn.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/goxuswgch.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gyltrdynj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/grqitaone.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gezxjijgx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gqdjvyxin.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxnxjarqx.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gxepsatdx.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gupibfpxz.sHtML


<!-- 参考信息 -->