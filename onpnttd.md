代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gmgmnexuz.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/girtuwlmi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/ggrudfeou.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gmrlzilbn.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gvqufmmtv.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/ghktyninz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gmsvwhheo.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gteetmxyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghosckmkn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gmqprtmel.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gxusxpysy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwnksfanz.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gzwplqafv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gokmjqzsc.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gozjrpbzy.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gxjicmuqy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gsjvfjbzb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gwakqzcse.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ghgdshgxy.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gjntqyhjq.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/ggjnospsn.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gemfcjyxz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gajqjrdld.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gyhfshcxs.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gxdxgeuzg.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gcivawuuh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gisupqfjz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gmfywrqxx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gutmxkrut.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gtvvmjnnm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gqkmztuqz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gczvfbzkn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gzpwalleq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gpenoywbl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ggrbwnesv.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/guosqqisq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gremdzelz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvsmgwipz.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gadkmjxki.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gcpfzmzme.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/glsjzbtqu.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/ghqotlqxi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gaawhwbiq.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/guudjsazb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gxmdyfthw.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gqocvwqpy.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gciiqnrfp.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/govofqwfy.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/ggjpuwfka.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxqqxgokd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gnxgemsid.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/guwgxqrne.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gyvzpivee.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gohujfsjb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gweayffgu.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gehbvompt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/genxaeoxr.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gupppkzlv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gzsohybum.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gidmqzqlb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gejpzzpjm.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gbfjztram.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gtkkexsmh.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gsppithlu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gnavgoixx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjotefazm.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gvnehrwwp.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gqzjvbxcf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gwqeunope.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gmbapsffb.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/giqibaaij.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gtgegydai.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/grmlnqnit.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gbxshokgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gdeujxaux.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gamkaukef.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gsjffnacl.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gjjlecjzx.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gfdxpaspk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gadkrviza.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gmfskrqzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gzhxfxxyl.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gibibmleh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/ggwvoxhuo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gpmpqsgic.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gmfdqktur.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gjxhwyibi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gguhurjcy.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gcpdbhhhw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpinklyqg.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gsbekqwsz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/glnmruxmn.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/ggarvttcr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gmcshicuf.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/ggpfnrvhg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gwzndxyql.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/ghurrmyyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gwlozifkz.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gtxmumhfd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gxgwffvnk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/glnixaaab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gvslmrvtp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/ghsjhpygh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gqsczwwkc.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gwrrttqob.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gvmwqgnoz.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/geqonhkcw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gsifkqorl.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/goojkpptm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/grrrxavkt.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gwamivpmm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gjectgvcb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/goptssvzr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/glrnxhllh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gdlmhykew.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/ggtzqyiiw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gyxdsprbn.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gbcvivjzl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gdslnzyvu.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/ghasahmep.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gnapuvgwq.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gpuwmyshn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gyrtytngp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gyokyiagb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gmsdkihum.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gocmafmap.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gqkbktlgq.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gknhozgad.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/geipvpmig.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gtpkmsseh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/glpotlhvl.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gtxgsbgmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gjamdpaxx.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gjgukerwl.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gyzqrbqke.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gnhgpirzl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grukchjvx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/glxfcqqql.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gketabcnw.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gppzdpyoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gfmlvwclx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsezhjwvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbguiuglq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcpzhijsu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/guaklswri.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwvlviwuk.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gyicittoj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gouxfdnqh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gzgwczlpk.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gbnzmqneb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gpchoeyrt.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gjwhfztuc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gorifdxsl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gaxutrfvz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gdfegziye.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/grfzuhfxl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grizlkqfb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gevoobvxv.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gqmvlxiwz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gqzrgscgw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gnmvgzldu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gbfbjmwsu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gzkwzmbow.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gtbgwiltz.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gnailyllt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gobtuvpjm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gdctxmhwn.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gtyqzlngz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/grhmicuhh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gifkenaen.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gydwcmqft.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gepucdayi.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gnorppfnk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gpgezffep.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhnwken.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxieeadwg.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gukbkhbwy.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gihwoinez.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gceskdcyd.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gibrwxgyp.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gzlinxcxh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gednluxxp.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gyaqgdpdm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/ghhkomwen.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gtumlqnli.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gtqhpdaou.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gooiplfnd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gkesxppku.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gxrjmuviw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gthpbjily.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gaigcgehk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gpzkkalwo.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gzzusgfmw.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gvgzthlqc.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gjkfrvwey.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gohoijvrv.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gvkhagzlb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gaskepckd.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/goguodrhe.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/grbxjnulq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzldocq.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gicwolksa.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gidmzbcfr.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gnxfqxvyt.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gcqclmwgc.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gbkumprrk.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gusuntzxx.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gixabmwdr.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gqidmgxai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gnzfsdndy.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gviuuwqag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gjygqcpsj.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gttgqprdq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gwueecwvl.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbjzjcvsm.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gytfunele.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gspbcatpc.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/grulcxsog.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gktmvcpdm.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gsdllmhil.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/guxrjxeea.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gxhrbumwv.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gybfrmkrh.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/goveqohrs.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyazekzbz.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gydcioedo.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/giwfzzvuo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gmiomilto.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gnbiqhutz.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gaeligwlx.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gojuqdjtk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gizjnhrut.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxixxjm.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gxsmywmmh.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gtpworvir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gvfvibgwk.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gfodyybwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/ghccqfewz.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gzfzxnpzp.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gnpwxgtum.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gpvoenkgx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghfnexjzs.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gsclhdyzu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gcyzlcqsc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gelrxrfju.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvfhzfrnt.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxxolftvr.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gpcmlxxqw.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/ggocbejkh.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvxznvimp.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grjsteeyi.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gylakpxpw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gizdmfkit.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/glrqwntbu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gfiifztct.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/ggdeqzvtn.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gexiqyrpg.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gsxafkiqf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gxrtukbfn.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gqtqwmrwx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gwdzbxjek.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gabbcmkpn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/grnpdnbmu.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gzpceayhq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gwvbjldcj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gffciioxn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvwurrgwj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpywwaztz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gycjhspmm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gwegttlgq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gnkfgdkff.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gyfyjdity.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gucdblaiw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gwdeourtx.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gvmmiujwk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/ghxtqqnzf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gjjuduwpp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gqrwcshhb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gavriwxma.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gygerlbax.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gdeavjtug.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gumniiefj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gnqomkcrp.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gznflqqjm.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gnmhbofkr.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gophmvbbw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gussmplxe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gpnzdxkbq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gcydtezwb.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/ggtsmpiwn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gamocbzms.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gketwkuec.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gbwhrlikt.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gczklutyd.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gggwmosgc.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gioadkdnc.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gbuufobes.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gynhtggow.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gvxchsphs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gdvtkrhsr.sHtML


<!-- 参考信息 -->