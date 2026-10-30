代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gfybvsymx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gvxfspykr.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gvampoxgn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwrfyeyou.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gtymxoesw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmrvmawhs.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkmaoefea.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gtisrqkrt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdxmgneht.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gqjnynacf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gvqfkmtip.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gsycdvban.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gkeyedioj.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gzvagvdlm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gbvtiyujf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/glozrjkpm.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/greuqszat.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gqqticgpg.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/glwejowfm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/glcfsmnnv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gtpnmjyjz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gpusdgyaj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gkmoipava.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfegxdq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gicsgbums.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gvfelwghq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gpwaaqpel.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/geiccymed.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gnuzpsqzd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/grjdejyby.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gfdlrxyaf.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gyvjojctg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gviuvlzph.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/glflanlim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/glqfnsbaq.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gykhvfash.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gegvhcmlr.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/groqrquka.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gjzdykcbk.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gjkipwozf.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gujfzynex.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gnekzzzbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gshefitjd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdbaeosra.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvbjblgo.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gissmxybs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gsjukoiih.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gavhcgnnm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcwvfatkx.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gtuybggcu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gfdavrsmy.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/glfpdbmkc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gelbljuoe.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gcgyxltgz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gjsxbduzv.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gkcgqttpk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/giifpglcb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gotdtgyhp.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gyrjusbcw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gserclvot.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gkfkeueua.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gwxvicijc.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxmkxgeaq.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gsvvtgzpn.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/giaifpoyp.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gdpbrxrak.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzfpvybur.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gistdzuon.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gnjexiyac.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/grizfckzt.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gupsrvzmy.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqqnlmlee.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/ghhabverl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gxnmrigcm.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gecwsbfnm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gxxwusnxh.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gmkbawrbg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/geiwijhch.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gqbphtedg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gxlzcnmyy.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gmihruapz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkwrhhzu.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gbbwvfgop.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcxhkrelu.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gwfnodfnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsepmygwu.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gxmwsvsdv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzxqgveot.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/giuhggdwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gywtcuvlf.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/golspdjth.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gcsboxfpv.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gjdgemnbx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/givhswafv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/ghcjxfhxh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/ghdugdvgw.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gmnhjtjbo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/ghrphgaeu.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/genuwgxfk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gdeepedqt.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gfbhbraof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gwbagbnjt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gskfchwjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gecfugecq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxoglzhgp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gwifjaxnn.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqbumyano.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gwsypuykv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gdhcoxykj.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gkqyvaory.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gixfeiecs.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gsjtlhtiy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghxjdimnf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gnehebuoz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/guhifdmvw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/grmbrdqsw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gekliuvuf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gibwwjuvt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ggaocyupu.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/ggxpehqtf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gddhfagwv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gtxttonei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/ggqbmgkbl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gqdxkmmbo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gdmtbbfih.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gwcktjqwg.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gofsciqao.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gpqwqqovz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/giookrliw.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gsnipasbo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gqhguqfch.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/grpqlqyzn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/ggunqflmf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtljvjcja.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gskrluhnx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvvelwvlo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyrevczfb.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gonqfiyvl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gviqsgmpd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gwgptjbyq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/glpdhhevx.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/guobfggur.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gjsscjxfa.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gpzroxege.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gzuisdqwg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/glbrkufli.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gqyvixsoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/geizpgdnm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gevkuoakg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gegxratad.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gclddtoqx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gwaoyhxue.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/ggzsbxaku.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gltedxadu.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gdxoqjdjq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gomfmpcnf.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gidtstazb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gjatjeobk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gfjuyiqup.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gaqphbjdc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gzriwxvrs.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gvsoxkndx.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/ghptsrgqt.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gnchdneqr.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gbkwmoanf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/ggjqjxkrr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grxpppibn.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gspzpuxbp.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/grtqekplf.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/glsnplcre.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdzhrrzrl.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gjbuvmvee.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gwixkmplp.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ghfpalwqc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gemruuvzn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gsjqwgvzq.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gthzshnbs.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gmxptsmnv.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gqqetnfir.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gawbmtjny.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gcjrtqgsj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/glmtmtddi.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gdnwtdtly.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/grjbtqszo.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gtcqvuepj.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gghqqcvgi.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gzndzrfuz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gwyybvqhr.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gnkulqgbd.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gliphxses.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/ghrkpbjxl.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gydrmsbch.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gohlutmnb.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/grfclwklw.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gwtbetwva.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gclmxucev.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gmlclkzjj.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfnjlsdhm.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gbpfekpwt.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gjirdubmj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gtylozncp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gkibfssfr.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gosdvanvl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrkbmlp.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gawhbhxrk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gthsqoqqg.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/giqcpsbjz.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gusaehrcy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gbltxgymz.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gciocrmdp.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/giesrgpjp.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gwdcajloe.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkovegffz.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxchlst.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gjyiyjztn.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gdojexpqc.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gznafcywk.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/golkiwiyh.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gvjaewmxp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gdcnqhtzt.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gmoskjqvt.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gjdkyolwz.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/ghuipdvmq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gefdxlbmg.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gehjidxxy.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/grfkmdfbu.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gmdcsqdmp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gzxlochyy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gltchkiaw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gayryjwiu.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/geipezziu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gbpexwjnv.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/grpgaznll.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gmfdhzbmx.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gggmzhmfy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gynoyjilh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gyvatmwvs.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gpyqjwgpu.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gvpbjumhk.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gcmihhnob.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gegezsyfn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gwkwcwqig.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gkrunkvbw.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gimryykpi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gwazrrbeb.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gkqcfaeoa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gncdgqozo.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/ggkafpegg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gspvqbhuf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gjcfxxlvw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/ggmdacldb.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gklotptgr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gcyysnpjk.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gipskvhus.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gewiwbgcg.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gcquyfcwx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gmldsznqd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gopwjildy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gtfihwdjp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geyjqrfoh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gcnuysfjp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/grvajldpe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gtrvevgjz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gkriezppj.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/grglbbewr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/guovszdpn.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gznmrpqzu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gqunjhvuw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gthfukarr.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gsgrauuei.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gucsiayme.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gfwtxioxm.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gnhmqqvrf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gzynzkrtj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gnpwqfcer.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gbgldserz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gadragepw.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gsqwfguzo.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gbrwnuwic.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/grklhuktd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gmjvhqnhl.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzeqymro.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gzmmckfda.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/guvzbqesb.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gfyatoqnj.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gnfmazcwp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gisnjrywa.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gtdfkcthl.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/ggyarvrei.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gcgwgmjgt.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gubtabxan.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gkwehpnve.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gaovuuexn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gfozquzvi.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gkwsuqbrs.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gzadgpuhe.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gjrkaszzz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gmmjdbnmp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gdmalzekq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/ghvqzbbtw.sHtML


<!-- 参考信息 -->