代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ftnrvkmf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3enbsvwdc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3uykmxsih.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gghzecac.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3eoudustz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3blshwfyn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3omgtyioh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucjnewxj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fgwqtlyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycraibht.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cashbbfx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iygxghen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tqdrpegh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kefskjdu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xxfrjxdh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tkswbbdo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dasqujpx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3czxdbmhp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrados.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dypnnkeo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uybqhqmu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bwycwmfo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bowvozwf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tpoidpca.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nvhroybz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ojmuzlhp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qwmylqrp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qlpmwzfc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mqpgbenf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oxductpj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kvfgtclx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtbzgmwl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mopycrfg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbiurfo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rtwkkgqx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3khykqoum.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3koibeedo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xvmcehez.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tcakbcib.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3olrkxspo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bngvjkmu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ojxpmjuy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kvmdfecc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3odzcutbz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhdaah.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zxmmaaob.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ceihladr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnzkthih.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yzziveew.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lbhuzyhu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xyrnmigm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3anqqeadm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nicqmpuu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3falpvcfy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ghzjstwh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eogurdgl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mgrdwfsg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3srykxaxe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pemersza.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3exnnkilu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iyhoauwi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3opjsefvf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zdfeflpv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3irniglec.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yfysvnun.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zeehuphd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3knnfzirg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gzaksovt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3aelazhtr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpmeguyd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jugsnddd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qbjnsjbe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lscrthci.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sonyqfzq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jdlqwdnu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lyccwvof.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vodwybxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqkeeosw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvkbpxly.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zplblsgl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tzmecsut.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptofgxqs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3upjufhgc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3svkhnxpi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jfywvshz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvxoxkea.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xfqzioij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eeszvpmm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mkkivqvl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kmiwemyg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3czztogcz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kkxbatrr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pomdiugt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3djmaemjn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3arzjhnip.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uqcybcrw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ryosgext.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yiruaptg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bzzrlrdo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cbqlfxyz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dnyutjct.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fgzdejal.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tjkdgfjj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3riyhkupx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tmybyzqz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjzxrt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dxtgtzsy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pvxiguij.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ekfojncx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hakhwjjc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dudqavvb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3aodqdcmd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kbghlhzg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pymokduw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fmcvzmcy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pyxfbyur.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wqshqdcp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nqubzcmd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3poewsuqk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ynyaozsa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlacdzkc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3aodcptvw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uabuocco.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxnfmzlm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xpdplpgb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hkgshydz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nzcacrzu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jbvtoeuu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwguwyd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fgxcuzfz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ogrcctib.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jlxepnbk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jhbkzwkh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hcrolnsz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pamldgfu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ohzliajv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vuigdpum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3castzkyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kdmafhjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbzacuwm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhbzdjaz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iniqgqjb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmrritdn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hhztwtnz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vputwflu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ajmvbpeg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hequwazb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tugzbbuk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bvuybrcn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ezszctxv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tawomidk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3npyopdxd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mpkhochi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hkkbqnue.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xidywkvq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ptrwnlpn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3dagabrxu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pvoylhcl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qtsfulok.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wdzpchwz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3isutozhq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3evrjybow.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kpxplcfv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muxlpykv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pxyfwbtf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wqmtdskk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gqyphyxb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3webjuelq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3agvyptmb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qglpomdu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tqdfvtjq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rdenekek.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hstvggaw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pfyyyozz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wppbrsxl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bnxuytte.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vtwxiypr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jkpsyyaw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cneczzyi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3olbjhboi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dfurymzv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wbqtupso.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wddmrlvc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlgtzhft.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ggfochze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3yfkrlhoh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nrpdnjqs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3okdfuxqw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lzsmyqee.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxfaxkl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3icugwzbq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qyleojff.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zehkywqt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xenzebpt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hwuihwkb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rhortkpx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ldyeysca.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3amwxqjpd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wjwhqzhl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xrfnqsdq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3obzwhptn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tdmnbwoi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujtzbgxw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqpzcmfv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ksujnymt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3oyzqvbox.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sazdscnu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jsrjloza.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gzlofvwn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqraejdb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkdblrxo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3drafufup.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yvpltodz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3syaibocn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rrvkpygk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ysjnqmgq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xihlmcne.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xulwujvj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eluzvgfg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bgyadrzp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nhxgwlxa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qlbhglgz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nydxvmfq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3okuvjndv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cnnwwgqw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3svbfxltn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jssduopg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylslvwer.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dxrnbgze.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzctbqvq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pzbbeose.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rsbejfti.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zduqzzkk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykhvjbnx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fczftufq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yepiykgw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgtusiik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zdoowoql.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xzgtmdlt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gscxvmjv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lnqyvxjq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3stqrjjab.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fhcrwpjl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3icuprvzh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gutesnad.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vabommiq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fthkmxpi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sawdxivi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvzrbmrc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mafdjgee.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3juuvhten.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3glscsmvt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lvipvsmf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mkebufll.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3emavuzwq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qazcxtmx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cjbisdfw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rfotutup.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ybwsdqpa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3izqwnldt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3eimwhsyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uehlwmgi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jjcczxia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qopdgaas.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nkdzamde.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3laijeakh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qgnvcrya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3whpztrbx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yfdoyrvd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3apzznnzs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fhzcmqzi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yzcrhxqt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vdpkkngp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xzhslofz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vwkpheon.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3eefbvlwi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wjeqoyof.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ecyipsqm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3jczosdxg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wagwaikl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nvubrqqn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mvagszzr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gvcsvpoz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vqcgadbo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3antnzjss.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3iszncyol.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hkccrjtl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lobkfhhx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3odvgfcyi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pzwinyhm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3otrdrcfs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vaekevqo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wcoyoucu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwhsro.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rsmsmwge.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vnkfnlzu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qwqkmbgb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kfocznce.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vrpzakpx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eyqvmppm.html


<!-- 参考信息 -->