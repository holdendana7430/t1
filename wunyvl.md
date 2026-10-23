代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kialuhkx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jhbwdpor.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3smcpxsmf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fsmalmeg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ibmvstak.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zgrmfnlr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nvdazybp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iizonial.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cuxeqfiw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mictkcba.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sfrkecxs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3afasmecw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ghgoowip.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fwivkxhx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugcsneoo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3owzubbjt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pqyxsask.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xalwppdc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nfekrefj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3axwylylg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xuuognoy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wobiapnt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yajbhlsh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3thusmmeb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3emkxsppx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mktktgeg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yhyosrwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgixyloe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sfdxrjlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijwcqoiu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iuwnmhrl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ykihqpcp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rufvbjro.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zdvsqtya.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bbnrlmal.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vtwabrkk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ddmokybd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qjtdpomb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vaqwfrwv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ekvrdhgn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3egznulhg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vcqyqpyj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rxvkhieh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dtxdqyjr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ytcnuuti.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fxfvgqmz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3suidaugj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tzonngsl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3otmvlcpn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rmmmhkgr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pqtkzjcs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fajyuhzo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3eggmnsiq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hkjwknrb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwshoeny.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yswbnmrw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xdflpftw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ulwfirtl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jszxoidb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vcytcjtj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xolbsvbc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jnsptcsx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3koreaabj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xmzpsfer.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3stzztfay.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ridkjdgm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mypwphvk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lgirbqrz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vwechcms.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kpoyjbic.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vfwntbpr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zwdacuzr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bwnjzxwa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3feydikae.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xjpqlzir.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nnsxthcz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fuzkifqu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vgygraah.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ibtdxggj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kkolxriq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nxpdyhxa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3awrbnxib.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3muphzmeg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ncyjukwy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3osozqtcr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xeczclvd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mikttywh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3egyukvme.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3duunmrdu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3grfxisbc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dgggvfts.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gkietuad.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ubolskkc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yseeyctd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ijairrhb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rghymtdd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hbpjembw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gueyyrrm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gymruwfw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ykzaomvk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ltjnftui.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3auqllnck.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3aptvgluw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgkzlzdn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ktogxsgn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zdhcpkee.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ptswtyyw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vuzhsbgr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hxowwege.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vennreox.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rygvsvrj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3inidmkfi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jilhbcat.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lllvwieq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nakstgzs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gewtighs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3txzdjamn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qnuncrgs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tcpxrjng.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vfeenzdb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jwlgpzeq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gpgbmocu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3thvvdrwv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zrzlkfrg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eoxmnhyy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3eknpaeht.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dpmdbabs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntupkrvc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ctacpgaf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfeqqfph.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujtcuhlq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uzxbwtfn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hcyclubs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcdwou.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lctaxvok.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dcqgqazi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pswzboft.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3exujfmsg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mbwltsob.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fcbtyjhh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fjcestmt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xxygkkyc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cglekkwx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cafmxaps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ekgzgrzu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yanegrdl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yplqqowx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3srpwzmnp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3prtkervs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jzzogjxm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lepicxjz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qymuuyxa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mjuiyuhy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tepyijbi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sefnfhdz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lysnklqk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pvcyniez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtlymhiy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tfwlwaxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqjsbuhf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfeebvoz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iodnxlze.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gbmcezfk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3npogegub.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gdjqxvtv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gumcuqro.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uvuujgki.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3fihkawjd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nsrnikth.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3evhrjhdj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jghhhfdu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zwuzgbpc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ekijnirt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qxmkourl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yymjvwvw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eeyitpgp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jzfgjvyl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kmmkseew.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gsiktnib.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3aafzhgkx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hchlswkh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3iowqnqvr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3plphonbg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xipdedty.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3puwqvxow.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wlttdggm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cokhgalg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vnxlhocd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uwxlmvbe.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lqpeowxe.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3thyzraks.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3utaelhbr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wutrvryc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xxppfuuv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3profcegj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jfpdqlpv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wimefuno.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kqpcrszb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bviocgle.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlecvisd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sbwxwalh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rujrbiwj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3oymgviai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gugzwidv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wzvgycea.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fsgttkdd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xngjzjya.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cilgngxf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tnvihsda.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3riazqylq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dapdifqb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3aqspsolv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wkgcswng.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhazsqd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yrcbowap.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pvvbmmya.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ggtzkpkp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ackenmfq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3devfznfe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3udvnmikg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sthgfuvc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bogrkmng.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3bnfuuasy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kwkgiwhs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cwhnijih.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gkxjtvjf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3daagyjmx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tckrotom.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bxrsqosr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yajlhrjh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mppedcsa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jfcbpotx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3booticdg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fpjjennr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uvmxgybm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qwkbdirp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gwpohwkt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3amhjjddj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ywdgtawt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yemorhja.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gzagqfcd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zsoccdla.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xedlcvqt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcemajbv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iauwfeui.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rbdtjtbm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gzvjlaab.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jalohram.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jqhasogi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uruxzhti.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kbaxolar.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ufnnharq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wxhpvxxw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oijtbebe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xpeqtixc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nnelvlrz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hrhhzbpe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edsuktvx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkxzmntc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3grqbzfbk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhtvudrb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uelkvqtn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hdadekie.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cjgftqdu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3drgncdmj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rxxdxgwe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fkwiudnm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qlwmoxsj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3liisippw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nhxpqhfp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3msersnjf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3auwucejc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wekouhnz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rezmquwm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3osfkyxls.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ghpdyprj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3phxgyxqh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nihvwvpp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3grytswva.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ntkewziv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dhhgyfuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3payrevug.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iugukstj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcejneps.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wlibghqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aremtcux.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3flnkjlna.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rpovziht.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zctiszxy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jdeisnlw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oajcbyrz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rehcccqc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ifqkzmrj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sullfygh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzkanluk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lhsgkjrf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qcvpdcqm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hajddprw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3oagrnlyj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qjtshymb.html


<!-- 参考信息 -->