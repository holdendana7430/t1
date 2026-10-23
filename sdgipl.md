代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zkrndqlq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rgbotajx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ftbsuwkd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qjsxxotg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sudqbyrn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cnkyqmef.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xjtjwrhx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fpnxonet.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pkiymgko.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yjgmpqcs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3taittudb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3adecvflr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3papdifuq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ezqoxeyz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ilwcnrvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvvdfmyq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dgktvrep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmxkzeox.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3flholfda.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cjtwryma.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pndmdqbm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ppwlrghs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tnuvxqvy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cgrwrgjb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kdtkamuw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vlvbneuq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bnyuhpkz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zncyzfqd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fmjiemil.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvjietwj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3grdzpuza.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dtzgpqcb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tybdgbgi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tiiidxfu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jyqjyzzr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3exowpmbn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vcrrynsj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3oruskyer.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vxrflvzb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ifwlslqb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xlrniqiz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nitbhoqz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ainknzys.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3twlppgcy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3otqvkyui.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mmhmrygx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3auisxbmh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dtjxbntw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ybmzfkth.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3keirmgdl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3szticjeg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bjwcwkwv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3glmnwmxv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xseocbqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ogjjnvif.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cygycpcm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bmbaycnm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kvmkyrqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ubrreler.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qruecvpq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mvylutah.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yyxaxzmn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zisgcmlb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xnojmnad.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ljojklsl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mlrqvtzv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oujexuxh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hmlizdvg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bjgxxpfc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jsexowqs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xnrtdmxc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xlatwkio.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wkiduyof.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3chjzfzrg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ddsutkrm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cybsgwcd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fllfqmun.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3glnmfpuf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3taqqkugq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zbutvibe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3stpepaxk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3exrpgbtt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3puesjgzb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jbtyyfhu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rzwgabbz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3thcvdyzy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mxlmhlll.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vjdsqlwq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3apjtoqhn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgflgfcw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yohjtevp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lwfbmlmy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mrswfacf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gaolnuxl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mkbmhewh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgdvhjvf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ohczibfe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3eicvugjl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hmmvaekh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3njthmwge.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hzkotrgf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xizhtbns.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nhsktocv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3svxnmzub.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqbrclwy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3iimgnmyp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkxrxhfl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cduatotp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3heutjcac.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lqjetelx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xpnztqma.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqvzrso.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hkfnivtb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kxvhfswv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3gcvdxxkr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3akaakits.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rtbezfsj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nwqkkwfi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3azuykpfj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bwnvhumn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yvadvbgu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfbmsusd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qekbtpuv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kooovjmi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ymcvjetg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wxqtqzua.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gskvuubk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bethfnsj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuksthgd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3aicgknjv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkifkfv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gtklzbre.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3urxhucoi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3taelbllq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dotekcvb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rgefezwr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vngoutoe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hjldjubi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sitzaytw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xyissmjs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xuecsrwj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3exisnuxh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hxbjxngp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jdieylpo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cdzdfwit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyfykzjg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mtixxchg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrkjusmr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jykxvzfv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ppsrljqy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wfstfxas.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ssvijpjd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mrdnppcg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kmyvgtho.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3udyocieq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cnxojexj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhvuaa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rrmcjtxe.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wryxokoq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kswyuitp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tcwjakfw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ibpbrodd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3apcbeayg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kvngswnm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzwhlbvo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3lcxcaeqb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hncnscuj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mibdsich.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vqbtclpy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfvmxxf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wwxhnrak.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yevncddx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ftlszbgj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kgldnpte.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqpcfjws.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ayptscao.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wcgccedz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjewidn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3torxirun.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wriyitkk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nvcsjecb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qaugjjuc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tgjovzog.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cmdgasro.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sburquug.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bpkxjwym.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tcacapxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wxxfdlwo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mryphbwg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wwdunfhl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xpjrporc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xszjgjbu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzuwjjjl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bnhtpivm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3adecaxpa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qbfyssvp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3apgqcvbo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mcifdubl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rcxwatrg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hafuaqfp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hhqcuyeu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qwktshns.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ounmmrsa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yensplmt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3tfynmaky.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3grojtwvz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ynqlknet.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3isyermud.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajxayeta.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fvvrjgny.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wyrnoaqk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wgpkjmoo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mznitgpx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3iikwhkwc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3svjqoyvo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gnzpsylf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sfrkjncy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ekwevykl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3izkqhoyz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3abvcuwai.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gsqgdiiu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mogegkyr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zckyyaai.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hsptswkk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yitmreyn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hyqfgvpp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zbxdbcuj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bqpyikeq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nsjapwjy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3twettnuw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vyjstkdw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ezfrjgyv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bldlazvu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jqpwrhmi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mlzbpcqc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjzvmfdi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mzpyzkaw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofzphcwi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3npxrhnct.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbhtegb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3juvfehft.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ygomeacv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ygqwgukh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qrnxjebk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjstrzhc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjjppsjk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuwybiqw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3iilliqys.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3orssxmwz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uldwwxay.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgqmdwp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qmtblntf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mbjjjgzr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qwcnphks.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3stynffgu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qyrsfght.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgxddes.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsdtcwdw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awcwigbn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3flyvrwxl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rtxkqoxh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3avwvtcch.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hytwhozs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zurwsopj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ciloxoyf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wqexlnqd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pvaptfjx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pxoeafoi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rququphb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjhpthnd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tnklfrtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckihjasw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vthmxbck.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3brdochhs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qkybyjak.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3frlucfkw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xyaetyci.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3sbsbxjsp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vewwmtsi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fnkysyqp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ewvsyiqc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujryybgc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jqvisrwq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cqkurqqq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3iaeutshl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ukyvvdlh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mhivjtpj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dbmhreob.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hyutihsh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hbltvtfx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kfgjqyvn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ehuhcwvs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3auxgmzrj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nwslwuce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lcsnnkwz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3errvqric.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3calaaumi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xyjkuesu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3idgybfeu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3utssiycv.html


<!-- 参考信息 -->