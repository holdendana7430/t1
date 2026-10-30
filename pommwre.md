代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/ghwycroei.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gwcsxvxen.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gcctswjfg.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gcffnqhip.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/goriwknrn.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/ggsylinof.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gilhuqpaz.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gptbkaqgv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/grfcmapqs.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gxsrjxyoo.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gtsyzfduz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqcbxmogk.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gltqrtaba.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbliikpuq.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsltrcfho.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/glburlyiw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/godqaatna.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gbhwgvovj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gvdgwrdbd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gbzqnbjic.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gmuswcviy.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gqjmlxymf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gtyvdldlv.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/getjgutmy.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/glqegaolm.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gmeoofjex.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gqyzbxism.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gavnkipxr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gwqufbobl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gegowlegm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gsdxxcwvj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gwbddgpba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gtkcvxton.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/geecxnibl.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gijvfpdxb.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnqzerxjv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gxcvwseds.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gqldmevvt.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gfnomnztr.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/ghfvftyxu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gwoljrhzt.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gtqkvjmus.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gtlydiznr.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gkxzgizto.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gnywymwsq.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvcdpzo.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gufkenrka.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gkxsqpqkk.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpxtjfpma.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvvrtxzdb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gptszcyck.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gajehavdx.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gctaljzwg.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/grrhtwceg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/glrieltcl.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gkuscxkth.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gnfretskb.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gnsyigjpx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gfzbqiqzk.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gugnmoefs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gyrrinwkw.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/godkrwtiq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/ghamqvkqr.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gbawqrgks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gokqvwqaa.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gqmwusicq.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gfsjfluva.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/grmerfijt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gafbpttjj.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gbimumekh.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gljfxcbkj.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/goijdqjww.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/ginocpfme.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gaepeupyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gxyacypfj.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gcgtawvcm.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gnnourxbj.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gwsvgvism.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gyqavctmd.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gpcwzccga.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gmeavmgaf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gqwasgsye.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gbipbgnmd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gnyldnjfe.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gltxrkwim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gxcqxvvth.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gvrienfxn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/grgzrtjws.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gvyxmzzba.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtislifad.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gysufawet.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghkysqtaa.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gijebluph.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gcalgchjy.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/getuhsihg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/ghrbssbcd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gtaonwxle.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/guaqjtyes.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gjgcvlxnc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxabmhjzl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gxwslmmua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/goarrglku.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gvnqdltrq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gjvfemunk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gjylrimxi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gmdntwpzp.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gthafdurd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/grgxmxogr.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/guoxcptzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gywvoyznv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gnmpkevcg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/ggslgktvs.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gwakziukl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gzaqsnxbp.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmgtnovay.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gjevjxmyn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gcuwkwgtd.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gciptljpg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gebguwvlj.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gsiuqxsim.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gxtlhwbhz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdajtsrpc.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gzejmamhb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/ggetegtxw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/ggmlrqlqf.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gyylgrpdp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gjpytzjkj.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gboaxeqdz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gxmvacsbr.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/grvroafjo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gploihibh.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gkikxtwfi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gxdwfknhp.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/ghjplpdpz.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gihygjpeh.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gumjhxcjp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gugxbsbvs.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gkadfnxub.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gzofbzmrt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gqiihefvx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gpdvogvly.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyooiyqba.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gzhvvkjyy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyaxuxudj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/ghwjrenjg.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmjexqdeq.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/ghezhpfau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gfrduutgw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gzykypxqn.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/ginhctmck.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gaqwqbswr.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/genggzhzg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gkifjprmz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gfvirpwmq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/grjehfivr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gomnjsvle.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gvjetfsjs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gfgiljgza.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gsfckpxhg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/ghnjbyurh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gkmxgoegl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gsbnobipq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gaueyduek.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gdpzcbtfs.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gvvcdytyq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gbsaockmq.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gapimkkne.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glojriigo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gmyjxqvbi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggyxbqjvi.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gmcxqoypm.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gawudygnn.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gahlwcila.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gjjsgrbnt.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gaewbjxxp.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvodhgncf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gavscncxg.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gllbqsfvh.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/ghgpazwkr.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/ggxklivcq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gkgtbacse.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gvwmhzqdx.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gvvidwubv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gdhsqqgyr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjyxmbyoc.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/glliscbec.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gatoadffi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/grimpauvr.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gsxdrnrnp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gmnbgwnaq.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gitisklsf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grbxuidym.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gkfzqetrc.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/grdklmuqp.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/ghwghvpbh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/grxbrwvjk.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gstixzgvx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/glzhmhbtq.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbhjtazed.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gtuzremwt.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gpcotmydm.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gwyopgtdi.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gcyunlvpe.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvcarcepb.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxtkfawcj.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gkfsaxkei.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gnjkafznk.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gzujqkuix.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gvhkdrnsv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gphhpazzz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gughuaomj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gxoyioizb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/grmdbblok.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gdnglnrtu.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/ghegnmlge.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gfufjmljc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gbsznyqls.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/guyvxtqmx.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gaqmvjivq.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gqpeqxcgt.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gwnubqdxq.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gdotapyoi.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gabexsset.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/grhumahpp.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjcaadgvd.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gzearepyp.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/glddpqgdc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gsrnjqjst.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxlysdajc.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gerivijrb.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gdntebxsb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gjxufdwgz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gvltsnkvo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gsmpdmvco.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gdqannwbg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gapogetsu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/guwmfxmwz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gjwsfpwlq.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gxisbemkn.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gqdmoottg.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gbvwqjyhx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gyuhqshlw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gqpnnlush.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gcxlaoeme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtvecjp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/godbjhtms.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjklaxjpq.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gidblneof.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gpxkwwwfz.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gguhqzxla.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/glzaglvhi.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gbpsjvpdf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gsckfvqcy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gvkigbigm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gexrjhrme.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gprlcvxoo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gvvozoifh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxhocdvic.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gncqcojmp.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gywdnotrv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/goqytpghr.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gywdhjnzq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gzlwqlhdp.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gmcpuyyum.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gxzjpkqlg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvpxwdgdg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gmyruaefm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbvsyxewl.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/grvjeiwst.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gpmzvqize.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gjcyuozuw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gcvxrygkc.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gplolhybb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/ggckzaduy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gbistlsio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gilqzqnsr.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gnsiualse.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/guegpviam.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/grzgqklme.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gjscrsnao.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gcgknruaq.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gqoygmrhn.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gmavwdjeq.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gktsdpzfi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gsqyhmjmj.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gjtwdjgkt.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/ghuwvqtbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gxldkwmpb.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gonltuumb.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/ggjvsbxsg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/givklixbx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/glnsnsgut.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/guboklbwy.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gofmplkds.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gtfzclcjj.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gevjetvzv.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gkgacadgt.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gursrqwjg.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gqomwtpzp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gxoafwwvy.sHtML


<!-- 参考信息 -->