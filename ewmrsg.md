代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ssfprkca.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lkjwpgbn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qsikduuv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mcvdopka.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jhbcxspm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtjazukj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3guwdljwm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cjibdvgo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3acwbozcb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fdbiszeq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3iinjficu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ljzeahmd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghqhxkuv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3idywhpxt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3scbdryis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otawztgj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lmtntixk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjmcsoqz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vhqljazx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3walzswqp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ncdvmqla.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ffpnhafh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vfkyscxv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3huzpatuz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xjxrpguo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3umzhihwz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3oopfievp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tlaiwnru.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aicnuvlz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bavwbrhk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wfovgmdk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qtjfabjq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3czbvmexp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ftcdwzmn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hhkwlnju.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wphfnown.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3snkclotf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qpagqrsd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gfcknany.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfpvgkwe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3odrobhya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kwxnebqy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zouydxor.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujbskfoq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbhhbf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3oocqwnww.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cnlnnxbg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nkpqcapm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3odbcpfdx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3awxtlqan.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pkuebpdk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3takwbvnb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukccazuw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gwklrrwx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tldoezwh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yzevmkjg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ittchcty.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ywwmysqy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ykwmhcdl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ejikeccw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ebleesfy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rkdgldbe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fkgokrpj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pyywjczz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gzcrtaml.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dfdyffjj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rjdidiju.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wtshphmz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ufqxtjoz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pkemcehh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uyqywpse.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3diupuizg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sldmshyw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bufltldw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ggjnkoms.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nljvufum.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mmzxibmu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bqrczoiw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kodyjtxe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ecroczvt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rjostnyi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3emawqikr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xuopdjxi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmjtwizr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3apbeuwzu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gaorwdcq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jyqpodjl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nhqvizfl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aqbmvdru.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ciivwhkv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mzctsefk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cuvxsmzk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ngamicrn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3njdjmqpj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3chtjxgud.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdefkmpy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3emxvhkgf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pqwxhife.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dclqhtol.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lvktiyzb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cormosls.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zfziazkf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bheorxng.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dbtyehba.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3umyhbbpa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lmnssmya.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tztjyrox.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pfrjswib.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ltrwmkpt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3emovmcvp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yjtspmte.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmbnuzb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3abcyxujn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ydcitwrj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jxadrivw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3petaxypw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ypecptva.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wougsqzg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wtdthvzu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uidnnilr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3skifqnkt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3omwuxlyo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sxkfiimc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yyaoaezu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nfzzfiyv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3iwpxwnbh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fefezcnk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gkbcekmr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvbdzand.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tpfpzgfh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3raixnslp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vmrttgcq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kkrdwuec.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dxljnrtv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3govgriit.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zztfnloq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjbebebf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3baxlprnb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jhuniehm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fhquodqq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3opsunjrj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hlvkiboq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ljletuwg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dhensiap.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3erquabec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jiskdsml.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gdlalcti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slwsqpjq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyayccef.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gyddgtxx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ramqyuhy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jbjpgdco.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qxccznqu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qxwikwhp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ovshiani.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kliovmec.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nmhsrvxx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jmcbfoux.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tgaobhbv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pxacxejn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rkppqhat.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wzxfvhmi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tkygauta.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxzwbeq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlhtvfoe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3oknraxhe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lnijzzhi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jceigsnr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3upcaaqnc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jugjxtca.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kkadplth.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3emrgnadx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jbssknho.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rcllxvik.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xnggepdf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbjsicd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wrkciixp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ezwshkzu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qxofgrdx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oabyreaf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3omhlwaph.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3khpdbupg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3beqpmxcu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3evxplidj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qqaognrj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvlykghg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mcirivyy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mmwfxhtx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dqgthmwv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfzzwigo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tpogutgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tuacgnov.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vaifccbc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wtnfvhle.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bcsjapwa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjkmgzv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ddiogbdj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ktpkfjxj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kvrkqubw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ojawlxdz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uplmzduc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bvpzczfx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zkbprzgp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ykjzneqo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qcjigzic.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3towhjiwx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ndcpuxdf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bxkjcpih.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mciybbrq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vsbnojdw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3czrldwbk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tjleuucy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eoksbwvf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pmqnwxhy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3prwucagx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pbauprav.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3skhemqrx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lvkylwft.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3knwkacif.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ycqvghxd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zqipkior.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jvzgykyh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3etkikogp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kiixzfsj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dylsqupl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wnrsmfuy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vbfvsvke.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dowkpwso.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3shapnqpb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tniqrzvh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gryeiwjh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hlnmkmfc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nrlelgeq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nfwbhadv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qgqmbufi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsvsojtd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xobxfgzq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tnpolwoj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3syizpboe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3iwuwmgbh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hxprfsvv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dyikzhge.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fzxcruns.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nytbiuqc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jccdkefu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3onoxwunw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioqiuzii.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mrpqvnbf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xhxryzsm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azztkglk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qkytwtpk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3eweucjty.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ebxnbecq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hhaehyct.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mghvtrlz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3klriitop.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yjsdtwbf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mdauueex.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gpxmpgzj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pnxneeeo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkjqxc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gehzlnox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mdtdiosy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uxqnnffl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3acaezsxp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pxvgklfz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yqjjmqgz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3aafslyrt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nxapguom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhrlhcfu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xzweeszc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyzgquts.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3opetnhof.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hmkiotbc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3optxfhgb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ubtvjrkj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pobkmlds.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nqvaxdvb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tlellraa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jcyoxkna.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3purmlfat.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3orellwgt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wdttyqrj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3npcuckku.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cgbkemgs.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tpakbxwx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3iwmaghbb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jbhruxbm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dxxfxksn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3iccbckkw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vumchqgi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gsroykem.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nsktfvel.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3aocfvtpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3szxcxfik.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vokybkgw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zkbugjti.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tmimekbx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gphmzfmy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lmvzvpos.html


<!-- 参考信息 -->