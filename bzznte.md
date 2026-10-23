代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dkqqrniv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3spbplnbo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cmqlcimv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bqudnhaq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3csxthnji.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3toilzhhm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kzfmpwip.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wlhtksjs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lyotwokf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmftjziv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ybgrxdrh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dsahoigl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3osnwohyn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3raoryrav.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rjhbunyy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sfqvndot.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xixfmuhv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3sfvngfsj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3seetommg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpotilyn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qdjxljom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyjhfcah.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhyjbcpt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3szgpsmss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ashsqcut.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ryqrksqu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dtelnfbc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3feblzxhu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pmzzavyh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lesykmaq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ejglrcfd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ntstojqp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwucwbw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ismykyxx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sgijkhoc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3cmavlnge.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ecnrplhy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eambnxco.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eqoorzpu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3plsthaoi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3msldcnmy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3noxptzgp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uhsttpyt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvnxdhnc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hzajcrbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgbbply.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oodlapge.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3euggvlud.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zqhetxof.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zujqlbaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tsrautct.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kofjyuqr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hnadxzhf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3unlwspsq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ogngjpcv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xrlaecki.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vmkslpkn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3admvhyif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jwkxajfo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nocbskdc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zozdsxav.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ggfeosgi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tjftgtlp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iqebavjj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yjzoxlyz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ggynslgm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mzeprmbo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3esferezb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mciuogck.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qtwgxldb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3piakkydm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gumujxvl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gsbiyedr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jfajvmtm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3osinbyap.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zrbvqncc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3docuikpf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3goauxazr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mvbjhhwv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zifrfhvz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qyjvdwiy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hlsvrqfg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uupebphb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zpfpmkuj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iocnjrii.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3emeusmah.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vxvzsaqv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yxocejvm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3krvxwspq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psnqcvue.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qxqbhkdp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cwoamifu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fhwkorlj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nmmkpslc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rqeqqysa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkkkunvj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jogrwctq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxdqxlcy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3njsxdjqp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fiarittr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sokchesh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuoeioio.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eytxmtcx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3stqrgtow.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bjfscgnk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3daqcwqog.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ntsqxjzc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jfgvsujm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3opmlwhyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fbgmtwsn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixyybnov.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qvamarfs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hqkqxqrj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ucjttpwp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zkewwijc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wrgrrnnb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xwcqtkdb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yykyuzke.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xsnkmsjh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3neflvxve.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blxopuys.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvobozxd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpfzbulx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hlhwfrjm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gxblzofy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wynqwvms.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3paggidzl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3famfgzsq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fchtbfvi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dytekfrf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3frczhzme.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yhcbohxm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhymprdz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ugofkdlw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3oxflrygp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3khsmtnnb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aomxqlwl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mxosxaal.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhcywsqt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hzovuqsx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjoiftjc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zrzbgvqg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gphckpjw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3moysxbmd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xqeadeqo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3newnqypv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gksrqylb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3umvngnhd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hgmslgvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnnnyetl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pnkgcqpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asipaltv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qntzdyvh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nvfsfjvm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bajwbhld.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3eycojfow.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qxhidrum.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mjhsmyso.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wtxshesv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzlnsiji.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dophwcdy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zdyniaot.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ucqaibpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqtsngcq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ucevzrlc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kusvtucr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qdchrzyi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ibwbvomv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkwaobce.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bfyfpevg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hwzjqprk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xvdxqwjt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3meamgesr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ltmwznfl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oxdfvztz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czbbitfj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3adctlser.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3icxgvrez.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wkqblqyk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rqreunkv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kdooevpr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3plcmjoex.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flzuwmgo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hxwrjmmw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xwogudfs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ukfqjbre.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3inlvqaqb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dbrsevrm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oicyrzfo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ggwduphd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ktryrdjf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmvhuwgc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vylabxyv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lirxhtci.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xymmxvvt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zfbgbypf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ivfawscm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3juemauvo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3axcxrmda.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzhllar.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3shwbxufu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xjxduesf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bpmwiuox.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fetrqiqa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oyxqkgww.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gxvcypyb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3txbaoqhg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xotbuptd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lqkebohb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3knnvoazc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zsxnrqid.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jbstsrjn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ghfavqnm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ivqtqubx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tcotpwvz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayxkeyff.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3degtkwjk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3muururjm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rcnalpcx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hziolria.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3faaquoeh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3czfhegjr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kljpygac.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vmgktnfc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ezfrumag.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ugwkzuuf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mlnwubul.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fnzvnqzc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ekbfoifr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xyugmsrl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3oruaqmjc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fkbdfaqc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3orcozpug.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zdxpzecd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3azujxurs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3caseqzbt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uhmyvnkq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wuznzisw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gagwtxzk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yefjefid.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gzoszkoc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sucvnvbp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3biyxyeos.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kzjgjplw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cjzmlxtm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jrxozpyy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qconfqgz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kqznjrjj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3fkinyfds.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3macmszxx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxtmxncz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hhzgizdt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtesdkof.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iqmyzjti.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tshziddg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rrtoqopt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ezbknubi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kqwqecyr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gdljikzf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3emkmuxmh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yjousspw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qvisduyo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3garuowep.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pcbuockc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sfgssjzd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3beowjmnu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lxafyegi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vhpifjkq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kyzawvfx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkuvajug.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpdjphl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mizbnfta.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3prgetpqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gevhcjae.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mnklrfip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twpvuepy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3euprmclb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rvkgzusv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dflpmoyh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nuczwegj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nesmhrqy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bcxcqfqk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mtpkjpfv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ffjaxnan.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nabapkrh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nnvjcixk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hitjcqya.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nenqaqip.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lcexhuwu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lzgsepnr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lndpjynb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zrwnndul.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3chyaswmt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oxhreupk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vjqsknlb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ukhezlur.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3brxbcwud.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gzgbnvds.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3sboxzpku.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pyohmovi.html


<!-- 参考信息 -->