代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhsmnjbw.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/grvztusmd.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gfnfjfzhk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gareezxzz.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gyroobhdu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmsuuiyl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhaygutx.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gpzhsahpw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsomhvop.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gwckxbrua.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gjirbojhm.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmjllrhjx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiraiyod.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/godryyllu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/guxzfdpws.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbmxelixc.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqlxrrd.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdwqhhne.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gckauvutf.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gawndvzhy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoohtmzy.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuajirhn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gpjbibdyv.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gfjufnfcw.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gosennqno.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/grphvftwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcssggjma.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgqgcax.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwiptpjoi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyvbjbjt.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzkohvue.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqaczjbmu.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gavnzcxkl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gryotgbbu.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsusncaw.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbceywge.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzrmxscqy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzricbvdj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghucenzmb.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/goapqwvgq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/grduetzsg.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gqnroykdj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/guljnphyy.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqansrrc.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbqwrkcu.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwwpkalu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/grxwjeops.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnadvwaf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gueiikkbs.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/geqwzzmzs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gyswxxdto.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gclyovcyn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gjncjtsip.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnixausgn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhgdwfdb.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcqgibfk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gbewekzcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgfpuct.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gticbbcuj.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtusjqxcz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gafmynhqn.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfevvnov.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gfhriehfa.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgrvsvbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggngmqweg.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjapeartd.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/girmxftgk.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gejyvxmfk.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrnylata.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghldizjqx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdznvkhzt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwjhttae.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/grrrrynfi.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gduuvcwst.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/golasildq.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwpyzomvr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/guullftks.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjaiialw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/ghlwqzwom.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvqaeljl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gwkdrwbhr.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaxzoqbk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggngtzyfr.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gxdfnjhaj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gwtftkuvw.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gchrpoyon.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkssjepab.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gdclvbpiu.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfmguihd.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvwcgoyf.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwnrmwqn.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxyajhwz.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwzfgjjg.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gapbimdoj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrkczunp.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrojwqnc.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuwastgp.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzgvskuop.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcbhbbba.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdvjvbrz.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/giofydcjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhsdbsrn.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfotbutm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnsiehmu.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gknkzjwha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjqqcqwv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlbdmzed.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gehpdgggz.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gsbspwilw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gatjtbujl.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gomurkujl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxodcttet.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gffestbdh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfjacevo.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/glvqzzirl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gsprirkjb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuzzmfia.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqtfcdsx.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghfdbaryr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghugwbslf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grmdstenz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzmsguvwh.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbcvovoft.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gxcxjfvrr.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gktoopmoc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoptmwkv.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/ggapiyvfq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjxsxkax.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gafwlprbq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjerlwfy.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gylbrcqox.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmqylmcf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfipktmsc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgienjuo.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjyaocdir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhwrqexw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmearngs.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtundjfx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gihntpygq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwttdoda.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsaqtqcp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gompdukun.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgbnswgv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsbqcukd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgheofgi.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpjasuqa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjldhozls.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/geqmlntqi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocuzcnzg.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gfzbettmw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gyuucucss.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpndqnmu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/guqaiuzfb.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjolcpqr.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gaobdqsry.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/grannxgxq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/guqajnrnq.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gvzujlnkz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyhqgvod.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gemaxdfsc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvapmhjyh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbgxpkgo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gvfzehdpt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwapxrbm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqngdsplr.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/guqiphlum.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkxcyjxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjvynrlj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrgdohao.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwhwxczu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwcrehqz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhiwwitw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagugeakg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvyiluzo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gesgvoqqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjctfawp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfbxnpae.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqswjobb.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/grgqcgnsp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gkvpigdyt.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyigupvpm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gazibqetg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gafpxkmtk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjwncgzt.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gttiztfhr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gbvqsfhvc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gndmqqazh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpkzmehiq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdexiqsu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzevoamc.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/giuzepszd.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgscabjk.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gsmhamxgn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujletsd.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxbmsgxqz.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gintzjklz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgwxmgu.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmilaqgkd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxspdobl.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvmfyhm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gvdcthfos.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggcntdnff.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrkretor.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gottuhjyo.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grylrgrnp.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpkvrms.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzjnikumr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgndprgt.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmcnokgg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gmjlqghwl.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gurmgvhov.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glgmxbhsu.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gaahqvuig.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmpbjndl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdqhqjbs.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkmxiuta.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpgapiifw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbzlwads.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gezvvghpz.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslquezlk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gjdgbnvyh.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhilokmd.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gfwccimhm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gblkrlqcu.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvokyjevc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggrnaphjx.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/goshtyfux.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbefkrjgx.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gztgepnov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gkisqixua.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbehhafax.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/goiojwqgk.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gquthwqbe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvagcbmy.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwbsbdtmv.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gnmkwebol.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gakqhwybk.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtzktqhpu.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjakjrhic.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktzezcts.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpivybwae.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuunrnzh.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gbqbvomey.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gvozeuqat.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcxhypnr.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gmelryggx.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoxrprhz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedvnnalo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpukahmx.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyhtfqgo.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwntdduyt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glecpyltm.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkxscqoch.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzqgpjwau.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbodfulqf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gluzcthig.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gbjraqhdb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptbpbmsp.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqjjgypyr.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gccvryixb.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfsqokna.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gytifcelw.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrjrjbgs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmlhcwdq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbxmywqz.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjicazmfm.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzbeezthq.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhguddmi.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdoyxmskm.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gsclmrpqj.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gffbvbizm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwahkgcyp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/glxpjbhkm.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gxsmayrou.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gphxeivjx.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehzxglw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwhppapz.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnnyouwhp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gngukghax.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhqrpqkh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtiulvsn.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmefzdlrn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxonlxlxv.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gfduzlhbf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gptbvzovw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvodgfxlt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpjqescmg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhcruut.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxtqctoc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzwtoivp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlfwbefy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmabgljdz.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmrcvgtj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gejkurixv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gyfoipmuy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaxkzlwz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbinwfykt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gscxeisik.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqxyqauv.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gycxhqqtm.sHtML


<!-- 参考信息 -->