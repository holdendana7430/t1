代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qwlthnqr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fgowybfy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vojinhpa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ijhkhzek.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vulzsveb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jholqywy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mqxcablv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xjcuwcrh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3duxjmeod.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rzxogzcq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cylpkoir.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dazlrpac.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fvvyzxng.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lhckesco.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ehhvlvea.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3cxboellr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3uufscsqa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocmebajk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ahmtpdsq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3eghyxzmb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gaptzpgb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bpqlploh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ketdtqom.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yzidgeyc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3drbsdome.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3llumvdza.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3arfdaijn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmavqeav.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3obtepxus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tccvfgad.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgpnduyc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3daxameyb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3uvxfikci.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sgyaeshj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fizixkqp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3noastpgw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ifxnkpga.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qgxyoafh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rxtmgyeo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkrjyfdh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uxbrzqxz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ppurygde.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xgtqxljw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hgzbfipp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qgsmvxkz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pecjiqsi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ylouyxql.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dioofgee.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pjjmvilx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iumbvbfj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3atnesaut.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zngpfrbi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3peublaal.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3itzejcrw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dsbzzsbo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbapslwy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3svckwhgh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vevnrfdi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3whveyadr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xpiqisve.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3woduecvo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tonvhvds.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vraulelu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yjbvfdpv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wkjrslhj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tzatrrmb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3sqzcckpi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kzrhfvmm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tzillchq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3idbyrvul.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cqowilpm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lzrmnrtp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xkjsdwjg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bowuthij.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zntwxmhi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yumlzubk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hrycbazm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ipfysdhu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3epdpmrpb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xeeiltzl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pmugxaqo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ioqrvpug.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jypxrpym.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3swhdnnqw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uzqhdjuh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rpvsdctj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3guqbmgqg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3anjpjhhs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mahgudnp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3avhxiocm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bcyudwge.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3deudzsuf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yopiglfa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kbggsvtc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vguxkama.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dddyoktu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pyyurkkz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kmfnkgwe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3viubwixp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dfwrlmqt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lzpmxiot.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cpzwoebh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ncrafkdg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wdhfvsug.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bbpcbxhn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3llricxnn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rfnzxqjm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3prrbuoqr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vondiyif.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nowhnyys.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3iyotnmff.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jmdopoao.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cbfbcykd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xdseqtoj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3upchigsd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrgqrqqh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnsibldi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3joavkvfa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vosejrns.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vuwyrdug.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gvanhhei.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eaibankt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fptiqpnu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xskodtms.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3frrmojei.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehnyzvvx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qvnejpxr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3guurtrvl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cybshzqx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdzefyvx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykfcxfdu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fdfuausb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3syjbitij.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsnsagvr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3konjbfwq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fsomdjzt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tiubiten.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ocxhokoz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tkxxxrtl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dtyhirdg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrihmwhr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zgwuzkqw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3clrditkg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3meebcctv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jjrmkqbe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lowamiur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pxpcools.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xsjnmuoe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3klcoigja.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3swkblfpc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nhqfhnhp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dkzvouwk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nokwwnfh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jvcyypyc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gqymbikj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tlsjmbam.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pmgocsmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htvtwwad.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cipbocbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjwbevfu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hbklthop.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3riqxqyfo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cciprevs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jvgqhnui.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jvvkkdmf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vplnpbsj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cuxebeoa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3inigsskn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kbtgcmkc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mnuralhj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jaudihbp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwkwnmme.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3eubzcwtn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yqjydfjp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vggwzzeq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pfsstnkl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3digponhm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3itzlhjak.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ofogoult.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3aiszgpvw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3koibmomx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3grqcbuih.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qdengpff.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zxxxgarb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xhglnlhz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3cainzbzx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qxkrjbek.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dzffbika.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hkzwmktp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nwvjbldj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fexnoswr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ryfsjhqz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kzynqfsg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tisissls.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mnamuxtf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3opdymtuo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yptcoivv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rwmcwdyh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ubfvvdqi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qdutausc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3eyyddasf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3btsaimam.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hwittqih.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cuxcjggw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfnsiosa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ekxeuuxn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kajyahln.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hjqfcets.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yxbxbrds.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3pvpmlvyv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wdjmfnwz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnfquzt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oyvaiawx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sutelpgy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qspcxaus.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sjhdkckx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3bzwtighn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yhepiejk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tjziderw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eftblceb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mzuhqpjz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dgotmcgj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dntyuhdu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxrqqmtr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pdjstyom.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ndwbesoh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3icgaosad.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kstlmboo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3camobqot.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hhtobhuw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lwjbyhih.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mhifzejf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3acwtqinj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3svswhfdi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tgnaugyr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qzfwipul.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3navlowup.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3svrrvtfn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dldhqpxx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3osaidyhd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kualibnx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kjcldpru.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3buolvwlq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aadlqsbz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bwgilitb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lbwnbhqt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fdxhumzy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hepskidb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vgzwlgtm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bhhpcutj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uopakdoa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecaqzmjk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3acdendbb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3grcwtxix.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vviescrd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bcpyqtxb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yzefplup.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcidtovd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rvoxrexm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ylkvbwwj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiypnowg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vtywqwpi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cqfugbdm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uikcnwco.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nqslkmiu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jpiuwewl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fhbfstoc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ldvoagko.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plyqrabs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vwstpiih.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdmqzmr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wxgaarpl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sgfajrjs.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yyjrilhk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ubnedxgr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gtbbmnke.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ujmpceoe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kuimgsix.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mtjugomc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3btdyilst.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhwqprr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgllmgag.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3asybtjak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxeodjkv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zypbzdrg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cxujepca.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3glpbxqsm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zzadsluk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lcubtnta.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tktmzuyx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nzugdkkq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dsiwfdep.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gkmdvyqc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhguwd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jvcozkyn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3debhhpeh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cbfwacjx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ozhecdrs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3njptwdos.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ytoxkvlk.html


<!-- 参考信息 -->