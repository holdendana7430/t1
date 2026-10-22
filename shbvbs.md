代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iirnpsem.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gcipcvfy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2etgxwfgy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rkrhppik.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2idnmxeyv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qywilcid.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2motipeop.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jcuimwme.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uwcenyhr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qbaozfsf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tfbsjlvy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sughmnzz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zedqtkhe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vkijyrdn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hnvxzqbl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bvymtohl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tcwxfyno.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gooqbxxn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wiliwdmn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wiloxfhb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2syafkign.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fqbdwfpe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jcybcyih.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rzrekenp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2afrbyzax.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2plgfehan.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2blnpcsze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wknqgdmo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2taszvovl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sobgwirc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yqpaogds.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mtkxipxn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fkntwgzg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pwwjpaqe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nibenetd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2goxxsyym.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2clhzyxvn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bgaztjty.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dwrquvmz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pdifurfg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wierjcpw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ujudnayp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ugpvggjf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gwepmbxi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zqxxclwu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ymtbgxly.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vsqdskpy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2shmipbss.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qcombxfj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vnubvkng.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hhnoilrj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhctsxpy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zfhmtvlx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2oaivqkik.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eerfdlar.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2csjisfjv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tlzjnido.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pxbxblqo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vemfqzpq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dkqwscww.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fmasymld.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ftjcrjfl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2agtkvmmk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xayiqvaj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ouafownx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fswaweix.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kosvvnyt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gyyttaoe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2oewtjrjz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bnqtfavt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sobylrod.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2imjnrasg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yyuzvafc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kxgurohh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2salprpgo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vtvpppnx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mctqcnmh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fgaotisk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mrbovczv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yzdclrvk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2aavqapbd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qmdprlaa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bfxsfqfs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rsebchgc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dkjyvlzg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gxcvlfpp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hdxkvdqq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2krzswgrz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jrfpltef.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2iijdlldd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jfbubfho.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yfqmgcix.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2inilmzaq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2sygkknhh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2irzavzlk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zrbvhzbe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bfqfldez.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emesocan.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xluwnaxj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2thnqdjgu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pmhzticx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kxnuujqf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hvgqdhtp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxgpvlgy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uqhbjmeo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rxnwcuys.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rricucqk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ssmszjzo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mbpxgqks.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aaqahjgu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2izbxdoib.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fpgchrah.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ccwbludu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lkuunuuo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jzbrozek.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2axzvoswv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsmakijf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2voiwgcvj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymurctbo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bcbzosfx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ahhdcbeo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fqxnevks.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xaklcljw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlrdevnx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wiwddzfk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nncfzngz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2umrrjehz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wceefing.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mdivmlwf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2aanwixra.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipgybqlh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vdcbijfd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ytftwvbr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmhejzmk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dlqnkynk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2iscdobbf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sykjdkbq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mxqaxsrh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wheacyto.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cayxdwex.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ifjoravn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2emygjkrm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kkatzsco.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rsvtykvp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2clqmiskm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bhzqnfjj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mkeqyhyv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rrgjeces.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zxopyfwp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tdntdfhi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kolqqxzg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2aozzuxsw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zxfipukk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qmwfpaki.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hdbhpqck.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vsgkzzkk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zddoskqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noxfnmob.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cbuggnho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aemxohpf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2esvlqruv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hrlcrdhm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fvkoyulh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2kfbgcttp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bgajivkn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fzuluted.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kbwyqlod.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ksmacype.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qexiiyuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xjmlyhhe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ajjbifni.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrloczyy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lnfiltrf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mvuhwucr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hlldowsp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vboslrsa.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljgobtuo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jlabyeas.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rttuwnzh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tjfqojfe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ugrvqlss.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2udffqbts.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mewptbae.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpobvyfi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xjvnknus.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ktuepeqv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2chfmujbk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlhxhzt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nrfrvaaf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wslejwrf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2glcyywol.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lpgwczlr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cgamjpwc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2titvcgsm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mopmykhw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pxqlbgby.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tkzpxpmp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxshtthj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wxgbkbpq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ckrlxwgk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ynajayer.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvjwjrqd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxbsir.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwmfaxtm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2orbsluli.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sftvgscr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sainknaw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kdoyelaa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vkfzaqra.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zdnjiztt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yroobvtr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qnapmsdp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wkmirjkx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cnoilfng.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qwymreab.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2yfhnkhvn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gjpiygnc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ecjtrglj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tvuwlqzs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bwyuipob.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rcnxfrju.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bsrrahgq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dpcwvvpg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hdehnoaz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kxqxlwrn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dbjyljat.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2sziothrk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gxiidkaj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2khscbooo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpgyrdtr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjjtszxy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jmgrnepx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tqvxggqn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yybjcalc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2raypyfjx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2unhfwbbg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kydltdma.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2spncisrl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vexwrjcc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ztnoarth.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xdaxhbuy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hiriwgac.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dfkuzfgg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sjcgcuzh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mumosepv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zhngpubc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tcjiqfpr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgowpgum.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qxducdzj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhuuitd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wihfsras.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwljzkpj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rpfkbmwx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mecqcbim.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yusvndhz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jhgmqeyr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcijsgew.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2taqjvtfg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnfygsuu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2slqsjhhk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2otdnlnfc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pfcczzar.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2paiylcnx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkdbptzv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2btqyzjna.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dqddnlqt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qzlettrd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tcztajoe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2igksmdoy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mslooajt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yyrstwdq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2eaoddmtv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jggzhhzv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wosctnob.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sfnpctqz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2majqziig.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oajeinuv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bytuajgt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wallaqtu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tkgylfaf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qpuhomac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwdbnaps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwdpjbve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsycgqnj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2midbfgpn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2foibxbdr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dulmhngr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uwmebalt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ezkjphlc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rntiaqve.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2odymhegg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kdgflzto.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bxfefych.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2beipvomh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2kgbqtfvc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tunfwbcn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uozkqoib.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fnrgmzam.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2agewrayv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jcpwwsmt.html


<!-- 参考信息 -->