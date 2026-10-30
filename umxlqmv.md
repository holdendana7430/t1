代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gchgyqtuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmvqmyee.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqbxcejm.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsrslypu.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gxbakyswx.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxnuvwlev.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxmrylxr.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/golilsxlc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gkkgsdfps.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtndylnbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwnkuhmn.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gghlqqnfu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncnjmpov.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjxxaqxp.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gejpezwno.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gpryumgsu.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmsgmlop.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpuxrxce.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnysfiotb.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbvprcsd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpbwzsmc.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkeifnkj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gindzdkla.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gomfysmnn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmikjlyv.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gticomeqv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvlkhygb.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gpnqpfokn.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gkymlcrcw.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiwuiiqi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqrihetm.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goriuziwp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxiwvlfb.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlbtqhyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gglifbltu.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gxizqjnwz.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjppgcuh.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/govxgaplg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkzqpgzpg.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gpwmbfgxv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gywdtqqmx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gdsikqxxi.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gnifxemfh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxtfufdw.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjvgtbth.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gebvytxkq.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guowdmimp.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ghhftqqrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbaevlcuu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckpdofzh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxqltafr.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvknsphc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxkqjgkk.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gapsvxbww.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnieasbw.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcpvqwax.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnucydpn.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gynwqodwm.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgrqvsgd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcotybvd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbavejvnn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/guukigpqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gmbhokmzr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdqonvb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtijvisif.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gefpygkog.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscisjjo.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlashetu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/ghkgykkpf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmgxobyf.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gsibnmrpn.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvjzyidc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwpbhqk.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbyhcyigz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gfavukzth.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcaowuss.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqrzowhc.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gswnyupwk.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/glrbxnubb.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiqzzbxy.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgmbibf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkamveb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gakiyupna.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihthzalt.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfwnjoz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gftapmhzl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtfluokh.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigktzjdo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gclaqisoq.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gprcqymgs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gkqaqasxv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqelwludc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gahzvlwpe.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxdqtevw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzdqxnhg.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmxqtbbyj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gbpvsdjuy.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gudinrdiu.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gaxtgtngb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gztowodae.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/glhoijdap.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gleouzffu.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgioqrqv.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxdtjheqb.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gamkssarz.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqhdlyts.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkosmvhpa.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkodccac.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwxtektzs.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gnrqvizzt.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwfmztcl.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvmneeix.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gdwsbiwvx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbbbodww.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/giowpxtqs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwvbmjzn.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdzjqfc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkzpguqam.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzabrxmq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfhcftfb.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqvssfjo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grmygbpoh.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgiqdhcu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuulysnw.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gwolbvbno.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvfypepwf.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlauztox.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grhnsbceh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdcnsxtyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gctemgmqz.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsiltnvj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmayifns.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkhvywdbp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvuaiymx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcvydojn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gnnouhupd.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/giykrfarx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gffxsjtgg.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gvngkrfck.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/giqwocttz.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxjrybd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gphnirvuy.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/glmrnphgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdkoaany.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/glvzicgnf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkezsyzaj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthujxppa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwpfdgtr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grnominam.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gklsixhgy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxhmkcym.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gtkrkauei.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgikwzqu.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gidkcdgby.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/ghcaaevfo.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gquyqxhcu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geswjxagz.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gyyukcbop.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsboofhdm.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grlcnbpda.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gembsgrls.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgpqetc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/galljhvrl.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/giqviqhrt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmrhcobgi.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/glahazgxa.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkehuebhu.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gsbfmivuw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvamaho.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gnmqwxqtl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gkiqeuqxl.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gfoqdotpc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozahztu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gldgglven.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvwacect.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyepoejix.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/groawbxds.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gekefomra.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guulzmzky.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gszghsgtd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbsruksj.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfvkypaze.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdngqkjo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/giuhguapq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaibaebi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtcxpamk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gacvbgmxd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpmulavj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gibaswwwz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gofhelaoj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gexzaamrv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/goiwtsnkf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaujjyvg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfxxgyej.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtphuaicp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwnxinoi.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/ghfqkqsxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gaibnanyv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjjduowf.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhlypxoe.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/geoyweklp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwrbmtaj.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gchmmuexy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqxtlttl.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/galaothra.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbtbudjz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gifbrynys.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcukezerv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejravsyt.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvmththde.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gudvygqrq.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstpuwptv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaeczwfg.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gskxkhmuu.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrwpiacg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gqjqtbllp.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpatmyzce.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/greotuccs.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gyjawnbsl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhfibbst.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnltlkzyy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkegykos.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnddbwsb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdkublay.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gieddjipm.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gagiltbsr.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gskcwmikb.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gitbtjeam.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gxszqbyay.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtbcyrrxz.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhbnysiw.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gbvwlivil.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gpihltlce.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhkugna.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gnywnwsvi.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjcuaxuz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpjhbnrn.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrvjkvof.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyzggods.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsndwiekq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginljzvkd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqagvpef.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxrmyven.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqjyhfud.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gketxkxcm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvbvxzmnz.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gemlqabcw.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvobuiyjq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzozgxhr.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gelkssoch.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfoxihjsh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpfguejr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmakgrk.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrjlwlmx.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gmaovexzo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcjfwnrf.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsrqbmtdc.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatzepij.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvxycdwn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxwifrj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grirkeenc.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhjkqwhd.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtfbhvmgr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnrqugzs.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/geuyeidmi.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gehxmntyo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbhfvaej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxexztrpo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gskuvmpll.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrmzdbk.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdnoluwny.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/glggtqfvp.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvyjinbs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzrtmcem.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glpubbctq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gztcyngua.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlqdocjk.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfovbgke.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/giihnavhm.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtpfbwlr.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/glszxraav.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuzemmyl.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ggquxrdpy.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gmozdpppp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/geyjqdufo.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gtokzxyym.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggessstry.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyasvdap.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozhyowsk.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gdjcteqfo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdbjddbp.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbhyoyrls.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gizldmxyp.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grwvmpmoc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvnmxgtpz.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/grpdjtymc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefzglknw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvetrvvej.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxjppbvyu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guukwllxu.sHtML


<!-- 参考信息 -->