代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pbphpqqv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vqrdpsfb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ghhwbnyo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wifbthee.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lbwomuyl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2eogodujn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2bfpkztsj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dygoxpgx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gnytfcwr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ygmwnplt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjefvnii.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ninqmqvo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2eanayvhh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2moanlkhk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hpwvnyhm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rcnqhsox.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jeubrczk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2usyanqzl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dcuciptp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qmzkpuam.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2yyuwifdm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lfbkqtcc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2psjetqnk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xrbyqith.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wdhccxmn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vmiucide.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fqtyxvdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izcjqbka.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2blbfwwyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbezgqjp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mxnbjxhx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2topcnrpd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2aivxthfm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2izketilc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wzwywfiv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fjomhuwp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2prxqxlzm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kubaimac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2azyhtcrx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2trsdccwq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2myidqsvi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dysmhksc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xgwribze.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ciwdvtte.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xyqzazsq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xawopmlw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kcpubwlb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vcptohtl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ndmjwerx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fpmddhjb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2unyqvprm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2melclqil.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pqosoabd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lexwikls.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uzsnoqyt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xtajcrff.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mtlqvtxv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ftvfschi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lpypqljl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bzkpvffe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cihbzfqh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bduhfqzr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pvhavixt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rixvenjk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sujsvveh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2csbntcwm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hxfodvfk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qggpwsag.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dejarjwh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hzldydvl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fxcrhcxc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rznitcea.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sgzdgbcu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qpjwqfhe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2pipkjmzp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eawiurgj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2suvtlckc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cdngaxkc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2akaiurkc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2auqsmbph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fqdgxhyb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dgdaiiqu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qoxgpxln.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yxnoctxz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2aboxyawr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2txstxvlf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qdktnbtr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fkeurqdi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cdnjfuax.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzfuzhdr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ocvymkzz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fqezfqpr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2crqeumge.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2czkzaijp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bgvnsiuq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nandorzk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2skthdmbw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qghwtgmy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qxtjrmep.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2usswntdg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iyygwkxa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2chwjmhyh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hjajrvvq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2alsslolc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gkxvaxqx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ggrxmpdu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qmdkemmx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpryoqdm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iuhljvwb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2faaohmko.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ckhrnedl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dkxzbvdl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yfxdrfmv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bpsdbiwp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zgmhoxks.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ilcqopth.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2plskvjex.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pdokwkav.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgxylubf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2btbcjlvh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kfbdgcap.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2facpegqf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lsdttehm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fzltbjtc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2apafyipt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lxntrmux.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qlklfhsr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2echpbrsn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zlisfsjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2unqjjsuq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ybiaztjp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2bahmwner.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ogseycns.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qurxzgwr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2axjangzj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sergrtjs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lemedeak.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kbdskbjl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2chsuigbi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nvhytvou.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghriyulu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fagktznb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2foufofvd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ndmlipyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ytlcbkum.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2knyjyogd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zwlxjyjp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fwpptnze.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wiozeipv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2knaxuomf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jkihcrii.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sjxonadq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jroqpafh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2oggqftyy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2quqcjoqr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mvygwgak.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wcktjwwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmrlacwu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lsxmupkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sprpngwv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2neeydfez.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nbbrjjqv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xowllxxi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pqyocwfi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zvsiodds.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wcneczdi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cxegqeyt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2evvwprqt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ruxzakrf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pajcljbo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fzzmekml.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmmnifac.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ibryqqjv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2djtfghac.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gacjguqr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cxqaifhr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sfskwwou.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vbfaclhe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vwzwdeyi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rlsdvkgf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yjxcuhyb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fmaprogx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vekilrbg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odqburiq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yfihhzig.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2eedhetud.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2evircgke.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nxwqgmwm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2feeyhmuq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nzvjfrlb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2emsmlvvz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gtcfnarp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxdmoq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zlkuajnn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zitiijmu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nsjrhufi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uzgnmimw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jbrermdd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2dbohntrj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xeexqolv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2spsahdis.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbreesjl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ppfkhhyu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ydagbqgi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xzcoenpe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aywvpyah.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mgfsgrbu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jhxnkexu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jajydjqq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bovvmxyg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2kplemxpo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dxljhnoc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jsbhfmvv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dbkqvxgx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2agcupfvx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pqxjurtl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xosbeptr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wobafzvy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vtzbsofq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fraxmchg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rczgiksv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2otnqzgcy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwvvqfzq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eqzgeibg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cymwodqa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2iywxfuyh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pldscxoa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2acklopti.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dvizhjei.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oprnbdkh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2igviiaid.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bwnitmrl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zyjjsier.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qspwruly.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pmrlzota.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2nlpqbwaq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2irtlviaa.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrzzba.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sclyoimv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2okavsaje.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bnsfjmzy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tpcfnnwf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jptalsqu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cweralqu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bgusytdd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kqvgjphw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2juebbcvq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jmdbytvu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzzxcvxi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhrazxso.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vppnrayf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twomxfmx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pbxuvdcu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmupaxch.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qhwwmraq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cmguhivm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwuydjhb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qpcobanf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mkagtevg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xmwizivg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nskuwkck.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nveqmtlk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxbznw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cspqjcpf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ctehlhir.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tltdybpg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2awslhmdz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2svjtfngx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kjmranro.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mzzkymis.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bozvofud.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pklmgtka.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kwdczyuq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hcbwgtok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmtfcgag.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kbejjwgi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yvtuhyyy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mtrxbpwk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jgoamnqq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ennzkocr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oxcvkgdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptnbhydk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtfgjsmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqsglztx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2khecfahv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fjvqcado.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2spflsjdj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pkojwcgb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2irwvzrhg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xeitnzjl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2phfcsnfd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tlohcaiw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ogklbanu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfnukibp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cwmgiwae.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2usafdvuo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dhadxcni.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2elgcawkg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gberxxls.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2quczyutd.html


<!-- 参考信息 -->