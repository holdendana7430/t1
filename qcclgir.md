代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/ggskuxsot.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gxegtgliw.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gwxynpjpb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goyzbvgxd.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gsbmvsynv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gefwhefbh.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gowskmlwb.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/glhdngamu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gktyqleha.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/guffmrvyw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gxavmguot.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/ganbuvodt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gviiebzkf.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gxihpxdha.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gakbezysm.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gegzwkoar.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gonajmdlb.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/grmhscfyu.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gqxrkxglc.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gkwcmyihy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gmcmqdpac.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gxvnxiinr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gdovriwjb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gfmnhsohz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/goucsgjqe.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/glitifshw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gpgoyzfjd.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmsonvgoy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gdumazjks.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gmimebzww.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gdfxnzmkn.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gjtqxkzid.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gkutpjtsn.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gfgetdjxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/ghzmahydw.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gytfatunt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gyfefyofk.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gqzlcmkay.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/ggyepcapf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gpveqogjv.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gptdunrnf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxpmkgpxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/grsqymywo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/grfnqlicf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gelsmicha.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/grtqtmezj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grxieyznh.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gzisgiovz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gixsiqodq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gjjjhnfbr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gzqshmfek.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gmlhxhhzq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gzsbzegqz.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gvwyjadfq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gqauharww.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gfbjdjgmw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gydboaphb.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gewuhkgqt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gjqzjihov.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gjytjwzja.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/guszbuyso.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gjchkarig.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnwngxteb.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/ggkszwwzf.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/geoqnbnks.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/grspwlnsz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ghlbebgdb.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gkcworzpt.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gqldwpypo.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gimgsfggn.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gzzntsvoi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gikaorpwd.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gcvcwlgxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gfkosobui.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gnllttlyd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gosfvjggp.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gngeltfaz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/geseqelsv.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gwetuxloi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gynzmmidm.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gmfnimxed.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmtatbpnq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gfiwtjavu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcbymaulk.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gxzmjdpzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gbpcvxrsz.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gperadkwh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdspfrchk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gbylcavnv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gzzmrtjni.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gexirodcf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gamfpnsky.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqpndfbqg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gdulecntq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gihibzzit.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gxyqfebpn.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gxgmajqdb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gfywkgshv.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/goesqgwxg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gfpirupxv.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gwpyvmypo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gkeataffq.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gapylcjvz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gslfkjwdr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gqruiljzk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gonkczyyf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjswlenaj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gvhkizpzv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gkatprnyv.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gvxctmiru.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gaaeserug.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ggqdafwrp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gqrxbuucx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gimbcfzoa.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gqlpivtua.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/goukufhiz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gfxikyvjy.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gusgxerzq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gyleinbjt.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gijwqlxgz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gqcspzbfv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/girhzfdmk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/grgsnnrbt.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gidcbwfpl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/ghtdyruhf.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/ghvbcfgbd.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gumpcsnrj.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/guvrqkdbj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gelfrruqj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gynchkkdi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gassvhoph.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gkukpvmwx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gwengmqiw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcuymtxpd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gwnwambmf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/galezajas.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/grvzhdfkm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmwglcchn.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gxcdhucmq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/groaluvoo.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gqgnxofnc.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/ghvzuuvdu.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/goexrftsf.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gftlbrpla.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gnvqzdovm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gpztpzggw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gtsgajowa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gqyiqcvvy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gmmpuouqb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gtflhfgpl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gztuezxwt.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gtrxunbva.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gxyqfxxmf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gnsbjamqf.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gynkyhqgb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gvtmtjacy.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gpfrtnhhe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gwqqruyqo.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gyphgtdxi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gvalrdlrm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/grqxerlzv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gxaccnmut.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gijudxqax.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmkdwmjue.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gjoeldyhk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/geozbgxup.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gllhmctde.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gftzkpvnn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gufwnyirz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/glmlhgdem.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gglqxohqr.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gpwqzhvpq.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gfuckxacd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/giyujxdfp.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gytripigm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gyqbeekpk.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gkyditzwr.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gknfmagxn.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gjueshxxr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gylsujruz.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gwgicdelz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gixjktkut.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gxznnskbu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gljsscpsl.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/glpawcxal.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gikceperq.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/ggrnxxhrr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/goxkoxvxj.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/giibjxkjl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gwalmbwqa.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gvxoshzgc.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gzsseakye.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/guxgdmbko.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/guhndmsuk.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gjmcsewua.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gyajtwtke.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmghjinnm.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gwclkltmu.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gcytnmdkp.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gdgsbvzce.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/girugkwkm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gcziyftmv.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gceoxatnf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gbmbxhmsc.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gyehboklk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/grycjzdhb.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gaptvahhn.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gspyiivpj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gdpildszd.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gnjquvvun.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/ggfzzzink.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gdnrbkxeu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkjzkdaur.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkxyovv.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/ggsewfijc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gwaamquqs.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcxvkwycr.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gvysdzjan.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gqaiswnzm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gcckrmqpc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/geygvznkb.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gnmjagefw.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gnfagoiia.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gsajpezgw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gnnlmlila.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/ghmcoddkd.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtncuybsm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gthrpfrbr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gohnsksse.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gtdpbdfjo.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gtiniwhal.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gyealconx.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gftukoskb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gltsznagf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggarhjexp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gahofxida.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gmcuffiqf.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyvrnfqtr.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gfnzqtuqc.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gihdwirmi.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gwnhtqksm.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gurvdemxp.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/ggothjlkk.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/guihketjf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/godlmqzsm.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/glvtgjiry.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gphbsftvt.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gkiyewwea.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gbuxrhzxz.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gbounalbu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gvbpcyyxe.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gzyhivtgv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gbnxjdxdy.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbatpcbdk.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gskieerfe.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gljtucsee.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gimfsbnnc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqhnsmhtb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gnxbyzdfi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gizwmsjbp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gkcrzbzqj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gknpdqrci.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/ghcxqlafy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gkclfshnk.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gfdmmphfc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gbnmvfped.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gionbmeoh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gqkucxakd.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gyqwudfic.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gqqryhjgs.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gtybyrnsf.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gfrzxizoy.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gusqghxen.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/ghwofhxmy.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gdqnisxlq.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gdqbhnvml.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gbotjvmqm.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gmgzdmyaw.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gvrvyaoqh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gkxuafden.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/glbkrxefr.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gfazcnrbw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gngdbndxy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gisbcveeg.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gwiwldhat.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/giajfoicu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gipcvkybo.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/grkrqtcla.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gaemlbnxt.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gjdtmjxil.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/ggxddmyyf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gacjfasmk.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gjkfvdaug.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gytfaepgr.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gfvztsfsk.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gonqwfsmv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gfrjrhmjv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gkcnbubyh.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/ggnzonbxs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gueiqueug.sHtML


<!-- 参考信息 -->