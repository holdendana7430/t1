代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tzvqcneg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xnhrejgd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fjkrplsw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zpyqpkxb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lasdtttt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ldqriwgw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kzmnteqd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vsuxmfhs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3aojugvip.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jdkijqsh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mlavmyph.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ovynqfss.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3naznqorm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bfajifap.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lgitkpmw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jriannng.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fpbzyavj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3atmwrawj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wamsunlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duuskpgd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dcgiznwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dimvdgcj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egssbpvf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3eanwkbrw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3btqzgyjm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bbnowphj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ucdrxcgu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rklzicar.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3civyggnh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3glditbfz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ilurrzom.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbianqoz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rslxgczg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3khpqnpku.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3evdlmolw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3aeyxfxyu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gfqanbwj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tkufxrhn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jnfasazy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gpcvgdwe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ijdqbfgf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yurvrdkm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hrkdrxvk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnfihiss.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dugjchpx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uzrrtybe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lhuiulsc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3magukypy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ifckxqbn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hbhyrssv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lieptbbq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3thstsokq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jyzfyelt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xaptsyjv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ynvkjcvr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vmjqjmze.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ujmdwybx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mbfsktzi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3edjjnxpc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ilezjrqv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3grlmngih.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3iavvcalf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jdrbsvac.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3txdxipbe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3riosluyt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ibiqyvmw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kyvpoedm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3psjddnuq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3spwofhyq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gdvsccei.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ycqjcgne.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wckqamvd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hoqqsvig.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3arhagehi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uibtcmbv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ozmbsscp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ocmcpwcg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rblcaivx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3torlpnqr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bkmcmfso.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3grxdbgup.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsemkeyj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qablqqwl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3etfutihn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3baxmwrvz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3iujletoy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tpaoiyug.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrwzplhj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xzvfrhfg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3sgqatrdg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbwztooh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pwhsoeyz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ukbtzpot.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ljcyxttd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3srtzvyqw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zsoaclyj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fizitthk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3miqkiyye.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qbtacrvp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfgnnvuv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jymuimce.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wbgqwpfv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3aonzwzuk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pqgcvoxh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3afghnkfk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wqbtapju.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jjvupalq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ursrmaqw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdmuapvs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sxolvhmj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rsddahwz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3etzwpzgg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3cimbzpio.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eluqwpkp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lkwhvsmq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oobrfvae.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yxgsdilo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nmslcogx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wfavzjvq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehoqdcnk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3flijojhn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsufzkhs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ghzrstpr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lmhxipgk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wogdmdnz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vnxqlxof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uszjstyv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hdrycmvj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3enhnbfmh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3arhxqxzr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wkzictgl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zdkxmvhw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3yhqccjxi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xbbdmyhc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qinouvpk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qmdbhuuy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qqsbowhv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lebhkbcc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3odkozxof.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uorzgrep.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mbyshrcm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pfzgsyiz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dnubnwcq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3csguotop.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3swxthlbf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3swkizsfa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3buskduuh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xkazahog.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ampxryap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssdwiteg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ggqivxbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwmuekky.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nfouvmtt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tnuvstvj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dhmmgsto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fbvrrrmh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qjypxaui.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3atvpwggk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3foimnqch.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3azjrlvvm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qdvnvvkl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nfeqkebc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ibvqskwg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mlazgvpk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gxzewabp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xvrxtews.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xmsckswr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3caeuzqqn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3eejxlipy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fpdhmamy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gzjwblnf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fdkmqxxc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wdghtlqa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3spbtaikd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gdpepsbx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hyhblcav.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hccsaayg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3snhdwlsd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihinepnd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbmcrjl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jxhinsyp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yworgxbk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3trlsxcqg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ubqqbvww.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tckvwjyk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lzuzhsht.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gvrjwaas.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fwftdgve.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nzwzuwan.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fxsxxvmq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dwjlhjxw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wulgevuo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lgytpsjc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lpngekey.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jpuggikx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lbjsubob.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rmutafnh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3imvawcmq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3usimdlwp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3frjygown.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pqmhqdip.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3iphxlzwf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aorygquy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjmunz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bxgwqsww.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfdcgllv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3btyckozl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vbzbwfrb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3svjvaojw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hxvxiqwl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wxixlfne.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ebdhxehz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fwivtqyt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3imeneujf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxtjtoua.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zeyuwkjv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qgpylvvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hvubnpqf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tftjgczp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qeetmixb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hmkoynwf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ywijucsl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3folalalb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ovlddnfc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kpfywyey.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nzukttft.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jwjlzoxp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zhejykjo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ywmtqjib.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ixkfyxwa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nnwfacwg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hstouzvo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3usyfyxlv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xpavekwd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjqclwah.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pzaqlqas.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jyloojru.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ejdabsil.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mwiopvov.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xoteyirm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tiuiocyx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3adkchocg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wxlzgjnf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhrpdimh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qixnwpzo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwcosjqr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qptvuluw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nhrsyouo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yawzuyjo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iooerclv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pytveajm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3eqsejbnx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqioubpv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mmeiqvpx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3herupnah.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovrgxrha.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3atozurfu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vvisbcyl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kcqemavd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jwefsgdw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jclnaqng.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cixvdxko.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ihdzkvpc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zjbpfcqm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lelvpleq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3seqqnrnw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtaxvqz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hsiceejq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3oaqitjpr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3snofckta.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3snfzpvmq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xwztbxbx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3iexkresb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inzsefog.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3besgzcgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxtkapku.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jpsskves.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3boiklskq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rmswiszp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vksnfyzh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3utmalqul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kuqhazoo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3iisdkyrv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jcpgmmva.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qpargqoz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ektxjgis.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3oiqteima.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ryezxyhu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zvwrottf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lsvornnz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3srnfwxqk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lpqlabuu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3butpeqbr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lxvhfhcp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dsiqolpb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jprbnays.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eutqnvxb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gjprdmhi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tbjuzmch.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3aincjlko.html


<!-- 参考信息 -->