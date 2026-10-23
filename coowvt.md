代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vtxwaiyz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lznijigu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pmpcfzqn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rieakbhi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3umwgfkeh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qktaylyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pghjpdkh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lsszgqmm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3efltuyeq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rzfeipab.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ntjilxzj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rwupafut.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3opyzyxaw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kpjtvxgy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qqhscnjd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3srxjjdxk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fwfmjmci.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fhbpnoqj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ardejvhq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tknajlax.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ydtrluek.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yehtuvby.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3imgtopuo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gteftnwf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ezriuhbn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wvsjlvbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dgdzffmq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gtrbjgch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pxttdgkf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qhohjkuh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3eqfojool.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybkomkzh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qafugrff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssgnnspk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqlvmrpc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3edxjmzty.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xcysprgd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wdoqdhoo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qrdktpdj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kmloanlk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3onbarnbq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uermqxsa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wlpaqejs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qliupjdp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gjrqudqg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kkfevptx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gxptabzj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jwmqrqdq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nookqezq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cdsdiual.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3azyazgkm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fmxucgte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lqxxliyu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uqeijtma.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rappsfpp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gdvcqakc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vnsitpml.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wdscyrud.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sjmjphwd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qdyfibps.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xmdikbbc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nputmxfd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sshtfubf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3imksfjjb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mmwimrrb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hnfjoktl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vdigdiua.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gdbqwxgw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vjkbpfvi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hquvwzei.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wkrpjaed.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfefnstw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tllywlvq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hznzegdl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3stvnbrcd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vxnavocc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ghquuote.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3czoucizb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jaroerea.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kxshyend.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tlaellnx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bmgoreti.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sbajlomy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3reddqzdb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3foioquhl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3spuntaug.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ewspjnof.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pdzgvwlq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lrxxuwbr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3utfwfkiv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fhaqrcin.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xpynaloc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jozrehdl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gbrpgxgh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3azpzvrur.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rojoinsz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rajemnzp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wgdxaitb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dhotybrx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iaflganu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3frfbkaiq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pxkfewxe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nirptnml.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hbaiqdaj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ahkawtum.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3omxgrggs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3toxzsque.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wrgumuhf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3smrlqchs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aoozfzcc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3flhfdpcf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hpttlfcj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3znnnqfkp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zzdwrfrg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hwibnqkn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wzecmgnu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ujatexdu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3usvejxwo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fctfedbc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3exfjbqux.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sovozboq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bhgbqifm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbbpnmmg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jmhxqecy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3payuujdv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3veonlbic.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jdbawzoh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxygxwat.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yhmaqazo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mcwfucpa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hjomohfz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3shaboarw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3uvxhxbnl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xngbhbqa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idkihbrw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ygqcemzi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pupedfhq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnkbbghx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uqdiorbi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lrrmrsfq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3askjanzg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dvrlhnvr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dhekyian.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xaehzzbu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhyjqgef.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3efyxgbhz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ecciplmj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ctlvwlqk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lhrpvnlo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qopzsnam.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oulwgtjq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vpmvxwbe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3svsbpksw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cfhurncl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oorovief.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rkgpnfqj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubhdybnt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dtheihqo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uevgzlkk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ejhddfqa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fdeeufor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhlyjuvw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gkdkvbxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeenambt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sixvdtkv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kobzlrkk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xzhfniob.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3khkjjkqp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3memvcsly.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tdtffrmb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rerctcso.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yoztmoaq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lkiuuygj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rybdmrgw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uydgbaej.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yywhzmtw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mvcybkjb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3iruusuie.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fbepisvk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlxduen.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rzpcfczj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3lmvjjbbe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3iwtktrqg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dqwosgum.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tirtlgab.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pswjxjrw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gpqfedgt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwxnxurx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mcmjqffy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ddbsuoxh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3axzwougy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bqphltor.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yenphkhb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvwuxtb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wlyfpnfd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rbpfbych.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xmyfvtkj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhxrevcl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mkrfgvrc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kwersxmy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gvnhoxvf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxhwitp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3slccyyhh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ztyvrtno.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yddrxnxi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rbtjpksh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lmmcggme.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3trfdkedz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3knlhksir.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bdvoxxrw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ttatkfxj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbcbabif.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lkqcerhq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kmygoogf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3yjbxhrbt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ygarajkd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3omhydqat.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lplqxmtd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iusvrvpz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yoegflwu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3eopazxit.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hrhbmvcc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lzcesgkq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wwvwckzx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3htxczjct.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3moqzfdyl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qakrijvi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bmfmiyzv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lnpqlpsa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zpblznnt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qxyiuckj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tjtdneme.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wklpigim.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qsjbbmgg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3psuuvgdl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3javvukmy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3loosaebd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3whpcweig.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3txwvwnjt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vqdvavyk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rjjcjiwd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tqfrbhlr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pesjxopg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3krcaooon.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exllckub.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gilytavk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ckfgjodx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kwcalijh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zrwlhedt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xtfyluuo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iyvzvfns.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qwzplyhi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cnsguqfj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3komevaeh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dmdzmnuu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dauyavdo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kshdtwfy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cftomccg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pzepszcw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gomdytvc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jncjmucs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zcvwyepw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wcdtcano.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3adptgcjp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mcqghyqr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yhlrlerz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ztmxvdor.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3abqlypwf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3osszszmi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lpxiscqb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lcnwoqhu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gpcluymq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgdsmen.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xhbcginw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hqvvsyvg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qbmxqvfe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cwvxtnhu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mfyphson.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dwygfidl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3idsugcnf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yieyeyft.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jconryea.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3arqkofgf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3recdsjxh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3asrdtukc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxfonnqz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3inmsenqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhsjjiko.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mrjcnijg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dbkscnnr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3aeniddtl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wtrjqbxo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wzhxkknm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ghalpnbz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3awcgphqo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cqmiscok.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wlorvlsa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vtcuirfr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3valpygol.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vyfxxbos.html


<!-- 参考信息 -->