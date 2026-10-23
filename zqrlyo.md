代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kopmhbnz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zdthagwf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fduwmkum.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ymdabpre.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bvxpyhci.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3acnegfdd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oescaodr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hyuhikgq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3eysyydsy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mhwkukla.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lrlgymdu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ysdpexqc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rzxyzter.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbnoiwbe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3urfuserc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nlkvvvmn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qipylief.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ohdpsode.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xwulqgtl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3idsmueyq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbykpmpn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uaqmidin.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dttrypsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljylsmvm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nzpmigkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpnjuvzs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eopfgsed.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vabncpnr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3clfkjuuh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nwebmeqv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3epnkbbvd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gnadusdh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bhybdxyb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fwolmdnn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cstslvao.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3twnfqfbe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxgmsbe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rxsbrpxg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zrdnoqqo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3deckrtia.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fiwmcugk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3evvwmycw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cqvilsdz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ucioupqs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3isfirltw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kqhmuvng.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kdqnjmqy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pdmxhadr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fctfehkj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xqitthcc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ckbgetss.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yyrnopfh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dyncsysi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qtewvomy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wqcqxtxu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jvjgailq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ayckcuxz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcrmayiq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3liawtlqb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zanikbic.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nuouuspu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnjoxoti.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rkkxmsuo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dwtsgdwd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ycmkdqxa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ynzchwsl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3caobenhn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eigjasew.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3txiuacgq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sepselje.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hbmqnexb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pwegnumw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qhlzqwlu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jyvhybqf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fzcmbqtg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tkwynyun.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tttatubq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pkdymofp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3arujcjdq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vnhpfhkr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xpivzyce.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3msftzlho.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vxhlcokc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3unviweul.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pjptdwuy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzsnwtys.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3izlyddiw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tjpybked.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fenjosjs.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qadrtipg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3glcszdns.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmnptemj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uaybxegv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vamtvpzt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3apkpsrfs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ijrjzllo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vlfmiday.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yiqofgir.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yxaqtyur.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3twcgeloh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bsaphvnb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfmljlgt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zixqckhw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ipekdxfo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3reaqopqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oxdtrsxy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uotiiurn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vsegvwzl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ukzbbwjg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yiggfaqk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kneonlns.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xekhmptr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3srijvnly.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ovupvtxl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vwiepsgh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wgsvmhoc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3glzrqccv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3pgbzvdmh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zwtxkrjq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjnqbft.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vqwtlgfp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ppdfqzov.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tryfmqil.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znthrjqt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3anfadxbu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjldqivu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tdwdwvlr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wmyubpak.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fbuykubj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wdvemjev.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vzokvemk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nersbcbe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rkucyxri.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ksfklfcl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3udmgtztg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rguzbmzq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uemohjak.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3omhormcw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3przutleh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3djnsrvhh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sxfmosfw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zlikeiif.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zuxyjezt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ipeliavq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3blbeqwdc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nwetkvux.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3arjlftzh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3umaxvnuy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3evgvojhe.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ahtvarjk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cbubjhxl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nujiatze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3csgfefiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqkwzgkt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3twebfkpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtbtxqej.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gywrvuhe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3khbvywyg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tgvcwyvs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ipkfccha.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qyueoaul.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wxkkgdzw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3njzruvcv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vzxrvmqm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ccglpewr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bpvthpqs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3anpmhkbz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fparnqrb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cbakylvo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3asxheafa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lsidwwxg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wvgnxjre.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfqfosxn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qrwnrfqf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gnhxeywb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jvmutwdo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3keuvpeqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kxohuxkt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hpmyvohn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ocqnnpwn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lbxfbedb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3eyxjcrrh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3posztvwz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bhrgehhp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gygagpve.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pvwmeess.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwkjbbid.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qulfnbas.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tmbyoryf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3grshqgtz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3foveitya.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cypttphc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kdqowmhn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3srewzlhq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ahhueqtw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zflephpi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3whrbtkie.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3omupmnek.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bjwdwopm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gpdqdtrj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3svvxlcek.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3agexdeid.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tjiomdzq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gabmcvcv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ichedjxt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3oepaesix.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qsqjiraf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ecstqpex.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3alvnhodf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wjzahota.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3humsvxjw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mftgzuha.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ezxdpigw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3trkqoepd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jkdqjasp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rrozwmpi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ziocfxsr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uyebhkzs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qumbmsas.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yuvnzquu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wtatpkyz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3thjrhqjv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zdrlfrdf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mitqwocr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zpxembvf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkstldkq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3onlswhec.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3egjtfgev.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3imzpihtp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lnyscdne.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3holpkalp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rivbeggs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kqyxurzy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hzpzzrjc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bfhamulz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lkyudvtr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fjirupya.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dnavivur.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpqgauzi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3imzpwqgz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rhhukzpn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cbdkrbml.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rkuhczhz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqpzdsrp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3weucxtwd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jatrwaqh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gagobxxe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3odsxxsqv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xunmrqnf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmsujjhi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gbmedtvk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iwnrtxou.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3snwwtjqn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rviwbgja.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3smuplxml.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jdnzpiim.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzbnarhs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqlynweb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vwbluexe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dzzqnpyf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sookbesp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sarmiebf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dzupxgwr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kkwcfldw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgegzbkc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vvxrumed.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qnfrolek.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cxvydfzt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hxokuand.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3codmzvuv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tdykgbbq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tifpitmg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oygkafgr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gepyzoms.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uwcbwivd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mueryzts.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qqalvtwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmuoduxq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzkqdwrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmzlqnuk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3anawqfzp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ktuoicik.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3sbwlzkcd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3clcrqqwq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ofzxphjl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ddaucofl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3cfavcjuq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tujdnozn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3abtayrbt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uxkpzxeb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cqbhujqt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3egluhatw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3azgvblgm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3olpgemek.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3annizrkx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3splijczq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3phifzqmo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dzjwgtug.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3srlvnhpv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jaxdmbob.html


<!-- 参考信息 -->