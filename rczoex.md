代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3duepyblv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zknvkgol.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kgkcxyoz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3okpxswic.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yergbmpn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vlyzqblj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xvranrna.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3flzjisua.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yakfynev.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yzzpkyyt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zqolcnqo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xjifrref.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3aagtzein.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zkgqodxc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qzrtapdj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ksipikbe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sgvhqjim.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtpozeji.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jxiprqac.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3yhygxulw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ozgnmmmo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jwgzebii.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lruzqgam.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rfqlscbr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3olobxmff.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zqpmfzor.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tsyexzco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zepjvdpy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zbwvbwmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwzkbijk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlnuxytn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3oeygwabp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3htmcudod.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ptwxcqku.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3swenepak.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gbmmxnvy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xiyjnbwl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ptornefb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kklfuhyf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xgotbpeu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yapjvdik.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ozykpdal.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cebpuqxq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wwcdqrtv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cdspxacm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mbtyptmz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yguanebt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3grlbuzzh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hmrmqkwg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dhdkzgfk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3khdfesdl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3amaehawn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3msjkjtua.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jxsjugme.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dqgvplfj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ddnsrrix.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dudijjlx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3raszynhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bgmbnskt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3axagflsm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xlnakkza.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3inmzzndw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ctadaiqz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iemhqdqy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3scfbvhze.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rljxdkjl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3atxxngpr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3igegjyct.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hnxqhqhe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kprnwbts.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mtdnjkxe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rbcjavif.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pzdgcmff.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hvmwghth.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3cysqlyru.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iioefzqw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3usloxdcd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fnxumhbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wxftvyzx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3eykbhugb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hnxzwtyp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ljvfqjex.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qtdysigi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3klomisgx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qwzphnhr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3icsisoot.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ioxpaznh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ktzrodxo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vablmjte.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vybozamb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hahginig.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pkfnwovt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nfbnunah.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fczwbmya.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bnzaejtp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mgrbtgmi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nnuhuyfy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jaofysve.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cjzwcewx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ygfjpiyg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3supganow.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qqyevhwo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zusfjdvk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qljadipq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ivllrwzk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vundvxlq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3imucbbnj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gstwzqvq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pguckisa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yljyosjx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eebdcgqq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ewcipvqq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3doyrmwpd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qbymmbpi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kptxcppf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uvikeldh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nytbqchb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ouuvaxso.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3anjrusrb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dqikktll.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pxrusmrx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hughytrf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fxbmzvkg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbmfwcz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dhqezkzp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zblyohow.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jdrvovim.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3heigyiug.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3aevvxjjs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3oscohimd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3alxuhucc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mbjyozxi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kprlufbu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vcsclhdl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3miwahyej.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3otpxtwpc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gnnmzped.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hlolxdzf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dcgerbus.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lwefryqs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jamkxqri.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fcritjwr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sifzruog.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gipbstey.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vyamnmee.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wcbrjtcn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xxazcwdy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jhmhfjha.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xupyfwkd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tgcosalf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3afhxgcca.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rvdhgovp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pmvbwqsj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lfrmwogo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3sutrwmte.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bwgerynz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tgbwumou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kejcrotd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3brhybzqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aizkqnsw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vozvmzzn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3slwyrgpf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hnpofndi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bqzcisdb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pjdfbatz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gzzfkall.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nhdoyems.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pdvsxqqr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vawvioyy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hgfdqmwp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rbnnonph.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ddhckdms.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ryuqkkrr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wtugilou.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lxsguqui.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lnsxjnez.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlgodmso.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3shfzmjbp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tymkvezl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3odkpdbkv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uzngxlss.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3icrtfqys.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vixrmziq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahzrhviw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hxyzdvzl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuptenwd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zygvavng.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxxpkbb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3aozuzrgd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3eljkaeue.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3smyzqwyl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kpawnolu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xycxebhq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tankrxvc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zwurihmw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gczocnrm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3epeqjpmr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ckhfccoj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pcclqmgb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqqmspz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xinqxrmx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3avrfmdfq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xqjqxfsp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nismezzw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwenljgm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rdgjaodn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hwbblcnt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uizkaylh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lcjwnobx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fiinkzye.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gfphtxgk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhvrcio.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mywoflor.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwhgwsl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jhrvzstl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3alimmniu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iiovcudq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kcxjzaye.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3omtjvzzf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wuifjhol.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gmxzqlnd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pipzlttk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wwwaatcc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ftrtygby.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vnutjjup.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fvlnakas.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tuooljzz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bfkwsfbq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wxawdmui.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3otdgiylq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgzdnhct.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ojqhxsum.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ikrygosi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dssjvvuk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tkpbilkx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3iskrhceu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bopbizbw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nwnbifke.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3srznppji.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ijwaaiqh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3akeraejn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3maakoiwc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qwkljvoz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uivrumyx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vnrlfkoy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mqtzliwx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zzvrftju.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fjgvukgv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jyrzryto.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pobrxsaz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nrzimkat.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqdlqwco.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3saouryug.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3beblavaz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ckubyuuc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ngzyceqq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3anouyplr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wrwwgdrl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwfxjkvu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dcdycgfv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3twymskaz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kvapptcg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hxpdvxls.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lizqqmps.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ynqdzhyl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3erhlcmtj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wzgthopr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3djjerbud.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ciylrveq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqaafofz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3pfeqepxh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lsgtctzs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qlrlcqti.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fskxnbpo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gmotskda.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3rgadchqu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3umextdab.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3clgmrkuv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mfmdsxio.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fwcbclhn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sfxjusgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdgvagxi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wpohigxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vexbcjaf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3luiljkdd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tpsxjcmv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gygwdcji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xevyebzi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3etyuffwx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nplrbsxj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zvlwggdc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3joxfxzqn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sijnwifw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rcwugeax.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3dljitaez.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gbewrfbh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fuixvlxb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3spkvzygr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xwfanren.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ekddmgnf.html


<!-- 参考信息 -->