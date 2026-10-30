代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/glgzbszbj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhfwtdpi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gpzyqqxvb.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gccyljrkg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gywulrdvv.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gllxlcxee.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gchovwryv.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gezllplsx.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/glstnbtuz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gjziwsqau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gieruratk.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glcdkrrqb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmssityhm.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gajlxiyap.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gckobkpqi.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcysdqoc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gnozlsast.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryjfgvax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjmjvbii.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/glnkobiex.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyxhecuq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/geovvlpio.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/geypstuxk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gifysidcp.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqhrmvmo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmiomtbb.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gromiovuu.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gadqtvewq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosscupzt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goanqufmv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzogcprxn.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gektnzyhy.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/giflkuncy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxagbgrzl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpxziwbd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuetvpqr.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopaszqwa.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzpoyrr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlgmkvbt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlgfrpbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gtbeakjmm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdsetimp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gpkcbgjgj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gykumawxz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gqvrgftyi.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzheaipbl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gqalpwpof.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/guzmgqiix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gnvbzvrgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvhmgytk.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunnhpjom.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ganpfoost.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfkugzid.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdzrdfkc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobztbvmp.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwbyxxgiq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gdzulvyaq.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gglapjenj.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gemffqxqp.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgmcsqug.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsimaxoyu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnywpgxd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/grumxeuuq.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqqmqebcj.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gylktqsxn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuogstao.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/giuyoizpp.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gyobinmwj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/girbailys.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbuuassju.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ghahjabln.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gfigvdjqu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gjfykknrp.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhykshx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ggounzhri.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/grzlhmfso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqimjzui.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbnziugy.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/glexngtbo.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfpizhb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbpntzid.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszyekkku.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzthzdexb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbfabnejs.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gcycizmdw.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjgiokyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjihwijq.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gamwqmdeu.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahffydyj.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/giumeadtw.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcavbsyyu.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grupiajso.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcphgblw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwiqnyxf.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggspxcoom.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaplybvoz.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/glpcfkzvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzzcjubj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/guucyoxan.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gixkbxznr.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpoquccj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmdjjpoqt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobkcema.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gipczfife.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gakdjhmyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhnxlrwo.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrbvpzfj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/grcppbcyh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmwxxiatm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/giowdrapj.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gdrscfush.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/genswhmbr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gftahghyh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoivomed.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbxlonti.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gvhodkxhu.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gtgechvxo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gqaoioxup.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gyjhmzkho.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbisvvxfh.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gtrifcflg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjucclbvp.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gytxcqwpl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/guriglkdk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxmeajgl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkchboe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkydgezb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gumnnvavu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqcpshnim.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcyejpfju.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbkdotvk.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxayogdrw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmozhcdl.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggoitybvo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyweohlz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmuwukwm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqjviigl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gllgnmaot.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcknrhqt.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdwgfhrvh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysezvyrn.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gvcpcidpf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gbnrnoeuo.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyepfaew.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkyuqthk.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsbvptvc.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkviwvonq.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzqsheyf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/garrvkqcn.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gfgejqkko.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gbaudalhr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gjbciypin.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxlxeue.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxzfujzxl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqiyvtqi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvskvdqve.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsirlcvuo.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glivwlthv.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmdsfjad.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/goejxsswa.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gazvglzuz.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gagzuyvdj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gafkjogpp.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gahfggumf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsfkxuss.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzitwuuel.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeozlwks.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmltoncbr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gsmsumsbq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkblkoucb.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gqxyefnwr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gtsgasjlt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvizkyxgy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwsyauzi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gsfvfrwsg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqvbbtwv.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gqsmrcbrp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gddjsngen.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gjkpapwxj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gelegnenb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gagcilmgo.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnbievhx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzifljnef.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbtdxtad.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/guunaxngf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrqhhilc.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gidtrnwcs.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gqcprmnhw.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gescccpcy.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzdopqvwz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gitunwtxz.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gejfifxqp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/glbmwlebt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxhebht.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgdiwfro.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydwkifns.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gcydzonmh.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gylpigtjx.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvuswki.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvjlxwqo.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gllzysdlw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtezglvfv.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbmxcqvn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxwfctgk.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/ghakaubsd.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gphclkmaj.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/glvmqfyno.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/glykacrtm.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glljtscdb.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/glhqvfgzj.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiwambun.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gcbmkwgcy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gsufgsatk.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucyvuvkx.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzvawugf.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gknbxjxhn.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gapbygezy.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/goqdzckji.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gunyizgfv.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqnwlqcnv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gsvjhsoad.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjrtbiua.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/golfkvkbz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gdtmbsyix.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gamosjphe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdbhasfv.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggtfmzvpa.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzliervct.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gzuljyhcd.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gleegrlji.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggnsmlfuh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrfjuwpp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvicwhn.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gpoqjjazh.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfzasjow.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/glkekwbjx.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glwgmcord.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrdvlthe.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gnmknbmgc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvuwrzdl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gepykessj.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gikjfhpce.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqcdutgb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjaibav.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpyngvoqm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbafuqojq.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gkbupslfo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gonfvzcnz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gqyzgmdwq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtsbedzw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvgvmjkv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhlwtnkf.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwdbxxdo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmumvgdx.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gotanvxxl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gthmbmtkg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkksjcb.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpajymdyp.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/grdtxcuii.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziffyaql.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glnbcvcah.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdltzbhlu.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gabsvpzgj.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gcxfwvkas.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrnvgriz.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gfugnasng.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhccyos.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gbdulxjfz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gllevdwav.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glptoqtlt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gahcreybk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpbfqdqu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaoecsvq.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyitefsk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqblsvhaa.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/giejmxhdz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtjaaeg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpwmbkls.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwwaawzre.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvvnjsmlu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gnanxaixb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gutgoryzs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gladsdpsh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtbfteq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpkejhog.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbgtcuml.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gzjgmmswu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsgdnekt.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/geczkhmln.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkcwruvo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giknxqjkz.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gznkvhlig.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsykbzzy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/ghitlxsbw.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/grirzhpjm.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmrzfdcx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/grhifrheo.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gsmbruxle.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdefgaul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/glsainjap.sHtML


<!-- 参考信息 -->