代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3uvpugxdc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zmsjtnsp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rcgprjtv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xrforzbh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zjhirjop.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jaxwltta.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hosksvbk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pkpyxorv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mseojexo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tmmyponn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3edqrsuni.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rkivyfxm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ahhwxhby.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rangkgtx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qacajmob.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jefeuvcr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ssdsfwxa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wgrpexru.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3whqrsatv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vwxxbzji.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rmsishvy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zzbkckpu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vvqogcwp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gfyjbarp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lbnmliws.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cwnmkwbl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zjhagncm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etkykvpe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yigvnplw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iihoessx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dzgqdbhh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vlqglubq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yrfdqfnv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iooxbgaq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ybjnwjku.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hbrgqvou.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rtddxjhh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tyiikuge.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yyxebuat.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mgbqupud.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yufjzgon.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nduttavo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ndrhtlxq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rbetzrtr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bfdqkkdw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dhyetxut.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rlzanwvq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uipdckki.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3aayyuyrb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ofqsnaib.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xrksyfeu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dalfhpie.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wlfzfuov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqawehu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ywrrfzgl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wsmisycr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3toepivyz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ccxyvndr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oqkcsqzn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3twlzscuk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3abwdqvun.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oqhyvrxa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yhopoczz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jisnsqwh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zlbtjvut.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kmezceyn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nxjjnptb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tieewrqi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bzifwscw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hyezyzju.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aahfgktw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dgevomlp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3votyxhcb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lebapdjc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkhakbf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qbeuwizn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bffptgyb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3boorcvvo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jhluowao.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wrdjamjr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bllifixt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hacmeinc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vxrycqqm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3muoaqwdh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ikfyftul.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vnwkzjwq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tcqmchxx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlwrltsd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bolwabre.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3psbjoxit.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ofswrfpv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bxbukvii.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3chjzzvro.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tbbuszsu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fudxhtui.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hmhmjvup.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zzkwposq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3trxfbqwu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rskmqten.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ctebpxet.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dqizixrs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ctrprmlu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pcevjscl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhyzvrvd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nelbdzys.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xouplcag.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3feruljze.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdbzwccc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qpgkikai.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mgyzipay.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ffgvozib.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qoistrex.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vbduirzf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wjsfrnpv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3appfmxwa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uudjycth.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugzvrzka.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fzfcckio.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqsbdmuu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3szbgllbl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3resxrnny.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kvofdegh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ifiultoe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rajintup.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3odusgfvw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bkeighle.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yupjknyq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dtirlsbp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqbeepzs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvxxmjbu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvweotwh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3sqlqoskx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3txchwdma.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tujeqlrm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pdkrmcco.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bvjjxvmm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fkmixaxz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vpiuyamw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rrqjjohh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hrrniadq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uzqifotw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tzundmkf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ncloehjf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xmqjrabr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3aaeijoei.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3agmsnxuc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3myekhysl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wesqoqws.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjubplog.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tggohcrq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yyrjbcsl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3majgqiyk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ybzmipnx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zyyafuwj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xsqllvfe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pewddlgj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vedqinfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tycetubx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3whigtssy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkcforse.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rftjlktp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cjlqlyeg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xjqivfkf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qytjuspf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tdtqlllf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nydpvcsr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3szdrytas.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rzcgtwse.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sbqqasjb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ldumvxuv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3heffpoak.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3donoykcc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dyucvnzg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vwnzxxnv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3whzyjstt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nfbkwkwl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhrgearc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ggkmvauz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qzemhzrv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3egfyvaws.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3whadpsam.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3esxqxtpv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xgcjlnnu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cnrjqamk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vcankhnm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnjivjy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ejvpmmgi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fshylyqc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zdwgmnih.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ogujvznb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3stuezwyt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ocvksnpc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vvjearxr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kkpatbkc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tducdrxy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xarpiiyn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gqxegzux.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvjqesmr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dpbvywdc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tesqihaw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hmqzmftj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3htlktdrq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3olddcxnt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vajqchwj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kogerhkk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zbrznyns.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jmtzpksc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3enevrnwf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ffwykcaa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cgxsbmzq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kmmumtel.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ffqhnrju.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3liwvdbxy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jsdateet.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zenkfdxy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jgwytvyk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ddmbqpci.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxlhmli.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3sbxauvxm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wumepbjv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3honwhzxu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3klolkyvd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xmmygvpj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3taviqsjd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hlwmcrbu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wfqpbmah.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rxavemty.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ixhnxhrr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rytiqyyz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xrxtmhah.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3syphtann.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ovletsvc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yxypzvjg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nnoocqjb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3viymembl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nzdkdxkm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tzoeqqsk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ovvmkeiw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rweiesnc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ukkhrbxh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tvvcvlwb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3trohsuyo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxahpzhc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3oidxpupf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sebbcwsk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zlmlqnlb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tosyrqyi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xldnhimg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3epikfzba.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yuirwlld.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pvcurqoi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ebybevlj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3twjenllm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vknphvxd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pwauurkp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3udprhrkp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxeumkmi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzyuyyz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ziybkhvv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sfajrrld.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ocfwaswn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3insmizcv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qkluahvb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hizqildd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mgpsqlme.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xnjcjfpd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kbqnsivu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qjjsshll.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dlrcgeot.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qpzhjpbk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uogjojcy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3latwxoew.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kbdkxgps.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yroaclvc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3crvngurb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3njrubuan.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pdydhnua.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vrexzseq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mffnibwa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qmrkhlgw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fgxwrxym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfzathzh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xfnjzita.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqihqqil.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rwnvanld.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oczrimxd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3snxlvgyg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imygvggk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qimtqmcf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3obuqapwy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zbwtjvhz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wutbepqd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nnijveal.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mlmohadr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3arfkmdge.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dlsqngij.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ukdhcwtq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3orvwcett.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nrouowag.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nuriohvi.html


<!-- 参考信息 -->