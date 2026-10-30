代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gqjflibkx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/grkgyuewr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gqzvcqhfa.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gxmfdvucv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gndsmlzfd.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gjbupgclk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gbstqmvwk.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gtrwfipbh.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/guargrnsa.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gaxrmfdut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gpcfoimzv.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gxnwactqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gfvhdqumv.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ggdgimsty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gwzfcbjnm.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/ghxbygzgj.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gtshkgyri.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gjamwlaho.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gdyxwbfwc.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gscdsquwh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gxdmmczln.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gzakyeopm.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/glyagbigj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghidemfmq.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/guooptbqe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjorrrsdq.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geghkrvsl.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gaujtlsyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gtoawembo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gsivxxjiz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gpvvtwhjc.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gwitkkcgx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gamraeygs.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gmykonhbt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gzbjgujzr.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gfvwntmnq.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gnpyesyer.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gbasunbpq.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gytfwjvwx.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gjnudmkqb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gohjivwre.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gqvwpwmcg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gojuflcvc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gfbpzymfw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gziaeeiwu.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gfeymelsx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/giwgegxbh.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmbnknekq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gdbkfnxgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/glhrambtu.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gtdprizlq.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gpwcpkmwd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwsgldoeh.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gqlrmmzrr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gneqkrwar.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gmpbousjq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gyzecomze.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/ghnvoxfcr.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/grzuamvtv.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gavvlqgsb.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/genamyyai.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gvvevbfuc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gkrrzycnb.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/grhuwoehg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/giqqoxuay.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gqzutineh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gyzkdkocg.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gqievqycw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghbphvjic.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gqnotbjdu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/goolaxirc.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gnxrfkyaw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gvoylimhi.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gdrfnzfnt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ghpujcgds.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gzsdhtslt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/grkinwfqz.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gxhhcbgzj.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ghdfrfedv.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gouoimjxc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gywxydlbs.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gackamhwz.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtvxntqpg.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gssalnwaw.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gukmdcgey.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gampdummy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gztpumeoh.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gsiubazbl.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gvnlvobkp.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gohuzldeq.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/glrbyjijt.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtzofqhft.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gfcopocpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gxjfxsvez.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gpxyajccy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfxdodbyv.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gydcmylbk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gwcnxzsks.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gvldcczrx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gbysniiqv.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gbsgqdsov.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/goehbzywq.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gwxorncqj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyedtqcjq.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gebckdtly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gkqdysirt.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gmbcmquth.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gmtdlroby.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gtzbypsbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gqswskrkn.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gilkjzwve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gemzjdrqn.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gdxtamvpb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/glkmgrgfl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/goskufxys.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/grfnimyrf.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gpfnqwmio.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gqrrbvcrz.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gpuukrjue.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gppwnmwey.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/ghwrogpwd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwzhwhs.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gqbfxwdpm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gxhrqwkdl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gjricmsjt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gccisibsd.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmnqhipqm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gydgdbroo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ghpolubxh.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/godxeqkwz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gsfgecfrc.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbvsgobqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grwxsycar.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gpwuniebv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gzibzygcj.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gbuhhmoki.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gcynrqseo.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gbtlelruw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gucnbqeqr.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gkczmwsuc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gxzhssxbw.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gyxsfclwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/ghdftgbyl.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gzdqsnmlt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gchqqnrin.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/ghzdcsrmb.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gfuiabemg.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gjhzplrjr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gfdaeijop.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/goyitecxa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gcgnkyxfr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/ggvnxzjxn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gkkunzwol.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbbrdwksf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gpwdqxdeg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwyjeummc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmsubvpif.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grxjjophs.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/ghleztsdb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwdmcatyo.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/glzyabamv.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gqjulgpcd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gpjogsxry.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/groesauzy.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gqheztlyi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gqokcgbjw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/giskxmqss.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gjialeqnc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gipfmxwcr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gitcftnor.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gyrsxdkwj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnrmtdvi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gqzjolfpx.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gzzqwmsqs.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gcklcaojh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfgvaol.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/ggmmnisrn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gyirkjojc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gbjmgovez.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gybvmagqd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gnlpuldgt.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gndxluxkk.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gemrppsto.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gmxzlefbi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gweqyqoeg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gdjcaqjrm.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/ghnhktjya.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/geimggeiv.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/guclspxiw.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/glarjscfk.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gqeabwbzr.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/godfllkqa.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/grpltlusi.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gauntzyiu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gwjbsuhzd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gefvzjfbm.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gciiragkp.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gwnljdttw.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gjpgfpkcz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gcztisdys.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gwyrebrqb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gxihtbwfv.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gfkltfnbu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkfrlypxs.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gmdilpefp.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gsiyvjeaq.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gxeikgaea.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gxtbsexyo.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gwsnahymz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gtoixbxpd.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gceqvidff.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gakievqqz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/guvjodhdo.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gmuqrngee.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/ginuchqns.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gymfdpbew.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ganysclrl.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcevzsish.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gllnpbsdc.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gyzxzjvur.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gparmwhxs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gfdwmlote.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gzzbkctyy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gmqmqewfr.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gquiqyilw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmuxvasmp.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbevyqovr.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gscrmzmsu.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gohpmkkkf.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gvdsttssn.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gzolhjvgf.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gijmvxtvr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gcixmbrxz.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/grluuanjy.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gzojoeskd.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gsuvskdtd.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gsvmpuvcb.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gbfcsahgj.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gjodtawvt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gzulegrsg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gxrepzuon.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gfeufjdzp.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gmtsffcgz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gbdfkgaoh.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gwtrknzyt.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gthciroxl.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gqyhybhyb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/goylpcwfa.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gnvkipakv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gptdyhqul.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gzeujskxj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gddvncqsq.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gdersqvjq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gefipwlqu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glmgrfgog.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/ggxtjivvi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gbzxmlqlq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giehrpwoo.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gxyxpdgcm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gokduqevn.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gxjsgrylx.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gexsbyzwr.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gesdfmdnk.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gznwslirt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/glafxxxce.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gawlesvds.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gwxxcxwkb.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gpgwsefce.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/giwcstqyw.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gwjbdotmz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/glwxpqfkq.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/ggxcrnzqr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gehqvqybh.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/geswzrlyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gryuhguyd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gkqrrhefy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gndgahoub.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzgfqrtvw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gjkbagyuy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gylavljpj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/glkjxxgfb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gjsogontb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gwsblaykj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gscdwqslh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gfbcmjlbq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gnihcpjoc.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/geusepxrn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gsvbhrchg.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/goechpwqp.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gpqpxyiol.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gjawhnjug.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gnycgpbge.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gqnozevdl.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gwmutojmt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gdrpmnmrg.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gucqcvqwg.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gtgcewgzm.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gzgnuovnl.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gdoxjpnti.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gvwaotrwx.sHtML


<!-- 参考信息 -->