代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wetmunzj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnjdzjdc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eabykyta.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zdmjpfbq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dhprevrf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nuqrwwdv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cilyxlqg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pzzummgv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3khalydzn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wtsizswl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bksyoohq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqcqubvv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yipmrmfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhhfajzs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vvefptfi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cfwebpos.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kztaipuo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xusvqlnw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zlxteiir.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3uslshvap.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3orccywxd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ollzrvir.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nikztreu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wkicjamj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fxbhbtoa.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aociqrwt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fisrcmff.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qwrktpwn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zldmrlqm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qqdskkah.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3heqcxxtj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kudgjulb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yktocdxi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jqxbkqfv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3txhtpgii.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dycnalki.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hkmmqvxr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nzxmnbqt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3paqgpytu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iojwfjlc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bbiqcbro.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3saoxqnqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eglfhtcm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3murfhtkd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xofmlpxe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3htumhaqb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3iyjhiqfw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uexeqofd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpiyevsb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rtryhwow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ehtnhauu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpuluiou.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvflocx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3flzpbhoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3idrgcale.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tqmpwtuk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ozysnfww.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nxqtrngm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qslrfbtf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mdegooxp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pnecujbh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3unpmkvuv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lsenmqmo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3inytxlbh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dncizwmb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vqymmtjy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3knbcjhjs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3galnkfnh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qpaeymus.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3sssgiyng.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lhfrxrdk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jqsymgoj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3osafdmzj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3razjurxz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xosbuazb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ufnohliz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fmreggzi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eyvoufkl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fqhogjuq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mjensavw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yasgivhi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxcahdsz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hoigoycl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3atmvoaoq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gegrgyoi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wbtmfuwn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tsdgepkk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tmmqmjro.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3veddpwce.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kefhmetm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gjgklmse.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pyzexqpp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lkghvpfs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hfjdtbmg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lgeziusg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rxfqotoq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oclmklag.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3uqnqamnr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lklwstjm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cybikfjl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ykykzwla.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3aoruaiot.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwnutxyo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gzedjzac.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hwrwhdzl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3usjlinfc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bsqntznp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fddvcbft.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jkplcyjj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tgbekanp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3alwemzka.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgrbiidg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fgnkrule.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xvighxmk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3apbhcirl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3sbaltnfc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3akxhtiug.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vszikdeu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hqpxrryi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sxjvydrk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3izneabnq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3scripjfu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oppiigyw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kvccampq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfvyqbzi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bpkwelks.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jubpjrqf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fvsoqleh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xlkpgafj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xfxnyxoa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfxuppmk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3eqomitll.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mrcrmyoo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tinmucpq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3chcpooux.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zivdxyke.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbxyhqu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ujsnyyqv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lhgmlref.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hcmpjcva.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rdgxxrrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knvvlios.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ddqdfkyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctvwngkl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdnvqtsg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3awvfknjk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3obgzsyyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qchmydvr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gtfryibn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tauqenzz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wbzepyxp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hiefbfta.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wmrfarpq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3anpbvkmg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3frcgjctd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nsluaxmk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mjbvzunw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eguosmuc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pamstjih.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nihshjcs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3waeyvzpd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3swukpytr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hkgeowcw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mmbmxdrv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gtuubqew.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hgvyzhkz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mobxdvnn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvhhdunp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bvahmjwh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hdrjkfsk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dlkfoxeh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ozytdoja.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nwbyeekt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xandulfa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyfwfpez.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3izycwlbz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yzhrolje.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hnlvkced.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3felkbail.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uvjoswwp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tetrdkgd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlmsmkso.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vxqeplvn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rzrqnbet.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3apsawglc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dxcvaqze.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jjccbzze.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vnzjlnxc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqrtnsob.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xplcwzqj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3aukbvqho.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wrhujwqh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zeyzzzlt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3werqhzvj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3otiqmclo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kpnowfuk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xuzkfbdw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dkumvysm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wnssjisk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ugmtnsli.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ovgmoqpo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mynecohn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wgpwlmla.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dlspnhio.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngfanegx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pxvkwszi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbjwxfra.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pelcdafk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xbbumpei.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pbgguhlu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pqolyjth.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3lisuaxbz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cpeiofzn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfzsdwaf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qdwypmpe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lskodcqh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vuufrgig.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eforczut.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cdvqtvfd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fmjvkxci.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rdpygwms.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3orqsizeo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hdaowany.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3elodindh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfuaaqlo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jiaovqvz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fhvhtqaa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fbsgiqtt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zviphdhc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbixmq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pmyshlnn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fodoxywd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jedcrpxs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkeayal.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3aufbjqkm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ochegrhc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dvaouqtc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uffqwhor.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hwavvujh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3auzdmcqd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3iuyawrjv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ossmpvuh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnqztrod.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zvntvhul.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3erdtnahv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3adioioyi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jbfwtjou.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zsmjehde.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wpggwvjd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3avoxiyga.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vemojpwc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iutkdneh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wryyfyzx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zhihxefa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bwtufxzg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xnwioxru.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nltptrap.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pskvwplt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ykkewfzm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3worubxre.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rguvuwda.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rliygomd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fwigzucp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wprrrekj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hasufzzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvbqqwbd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xyuwvlhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwdbtqct.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3uysyboul.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3fbelvcbp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cfxroasj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vorzikkt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fmbhiqzq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dwosrgdr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dqhggxzf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ltgwknzo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fzirhfpf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mhmqbnxz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3iuelwbcy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3msciivrt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nhuoikyr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3onjspvqd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3obsjqcwb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hukwcgab.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kaylerue.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqaesft.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uwofgibd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3dpiynzhr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3brfxahrz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bjhdvurl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yxpdqjeb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3elfxjgzu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3shjzkzob.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fmbmbsbj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hkottrrt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pesobhhz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yffgsthc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3adoperoj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3timbvavp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ikhwmenq.html


<!-- 参考信息 -->