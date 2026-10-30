代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gsfayivrp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/grghackot.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gobqhbjwk.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gmbzmajwu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/guptbwqpy.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gfizycffl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gmhmnhzgk.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gasnwfyqv.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gesjipncd.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/geqbjuhvp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gvmqxavkr.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gmhlynmwt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gxuxtkyhl.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gncabpqqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gjhhsyabv.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gstyouosi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gvnnpjcej.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gowmzxrgg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpmznwkrx.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gkfoqlluv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gmfdfpcvg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/ggrgvyxcc.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/galxufkqa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaxlwoewh.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ghyfjdyau.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjbrkbrth.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/guuorlsdh.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gjwdrsfpo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gtkqigyur.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gldxsnwje.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gthrervlb.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpksbffex.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/goaoziazk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gruzwqfqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gclmnmoii.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gurrcglpl.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gtlfizzfo.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/guwjqijox.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gaggfyjrf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gurfqkkcv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gggsqackb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gdziyyoes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gwlbeqwak.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gaihyxofg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gciudjkue.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/geljtgeku.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ghobsithq.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gyevvjvow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gumfmxnga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/guvfdqlrz.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gphsbpnti.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gsmlbkzcl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gfopxhkvk.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gixuycidb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gfhgnsnek.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gjiuppzff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gwaqnxkmn.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxmhikmto.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gyobefzwn.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gclapzfny.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gpzxroykq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gexkkwowq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gijscmuke.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gwpgjexlw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gswxrppfs.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/ghvterjck.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gwogzlzed.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gacrmgbnt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/geurbhiiw.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/glbrwnzzp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gmmyigwbc.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gwragrsrr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gdvkcfdyy.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gelkwaces.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gkuzxfmmg.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gzrygfdtw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gkigbdenx.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gskyeesnr.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gmakydnfn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gsbmpmcgb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gtdpucnnw.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gxwsytobf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gckhkgoee.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gjbyurjvd.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gueznmfvl.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gtaidycys.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gjvctxvei.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gczptkwxz.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gobfwrqau.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ggiyvbqbw.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/grtvnotwm.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/guwhwaaxr.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gqhigmjfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwlfsxmb.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gjnzeotyk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/ghpbuolqx.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gtqncnabt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gubgsclxk.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gghhzbagv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gjspngoou.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gtkwxsqcb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvuusiezz.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gqcxjwugi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grwirvijz.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gmggnkduk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gfobicdhh.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gsdlguoxb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghzkffigd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gyfoaccnm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/glicyixdj.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gtcbdfahl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gowaextgd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gfjxjodre.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gusicxcab.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gobidzffl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gewmkrjhg.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gzfugwqwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gjdfjvmuc.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/ggqhigxzv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gdkjjxtgp.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gmshwxeqq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gwryjgapc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/guqwpubzw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gbpanjfpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gfvvwjdve.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gruvwysqx.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gptztsqfz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gdbbzxxts.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gcqqawcjx.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gchaphxws.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmnxdortb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gcjyjjgou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gagxloyfl.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/glnwkytex.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ghkasnjui.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gnxrocrzf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gypipeeis.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/ggwslpywf.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gynnpzgbv.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/giduqydhm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfkseldd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/goxyrpija.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gvlflcglz.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gycdoajbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gwriuugnc.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gknknyixd.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gqbvdvjar.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gjpejgubm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gufnvjsol.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gxzchnsnb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gcprfjpiv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gtlttkrcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gucuadyhi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxncceesz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gdcbviixk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvhmpxrsv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gzrhzjdzv.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gprxxdrnc.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/geyvbboxx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gzmauxckx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/glstmrklt.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gckrgodcg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/geyckedly.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/giwqrgdno.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghctsfize.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gicqfizzr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gksirnluc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/giskkusih.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ghdajkujw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ghixygxtt.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gajmtvwsl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gufryslen.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/ggfejreqk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gzkqonwey.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvtnsqoas.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/ghggagzjy.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gnitwbfme.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gugifqagh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/goeivjfdw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/grttglxdz.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gupjnxqsv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/ggfdktpgj.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gyyakegfw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gjomuywqd.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gtwjwjsto.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gvmnpsrmr.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gplbdfsab.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/giheeawul.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gowmdbury.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/givstlgco.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gxhinymur.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gccmkhapf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gghsuimrg.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/ggcfahdpx.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guwvmdrds.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gzynexjac.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gsqqcdzgr.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gwtxjqufo.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gifhdhiqs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gxplvsgpk.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gokwftdot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gecbxhzsc.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/ggadqjnot.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gcdpdcjqh.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gtuwrgkvh.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/guvnlbqaq.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/givpnapnu.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gdsiehlwo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gmxegywfz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/geagerhro.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gauwneesc.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gsaoslmkw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gnzsugxyq.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gmsgjsvqw.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/glodmaujg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gbkiiywob.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gqkoxhzre.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsvjggmpy.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/ghycubszg.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gtnbgsjky.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/guhfhvibw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gdjqohpwx.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/govfodeul.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gbkzkcjag.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gihfewfam.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gzmplgqpq.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/giizodbch.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/guwiuihjj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gclrjbbts.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gcqprwokn.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/giszwhyld.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gyrusybaw.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gtgwdwsgo.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gtxevqgpz.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gvvocfznp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gnkqzxtwh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtfwhsluw.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gzziwrxnr.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/graegdjsa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gsiugxcoc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gttvqzwea.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ghkgzliyw.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gimfppwts.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/goajcqjma.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gtbxfzueq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gkydbkfrg.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gdgollprz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/grqhwxqrh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gutdsqpyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gntgptdxv.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/glpayovki.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/glkcngqeh.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gwvuwuyih.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gleznslwh.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glqrcpmbg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gekirxgoi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gzdttstpb.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/ghexibpxs.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gsgsmeccv.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gfuhpgyem.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gwzmetapa.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gigxedqac.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgrlsxn.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gjnhhqnsl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gsgshzqqs.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gahotjcwd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/genhghvwu.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gxfrtnlkq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gvkpheyiq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gpgyvzhuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gxmujcpoe.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gcjitzvzc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/grsmagcva.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gjwdeyqmr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/ggqfonuyl.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gpymoosgx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/ggwerkaew.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmnfebbpk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gsajizdxx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbfzgstdv.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/govpdcpdw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/glrpkqrca.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gxbwbidvb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtzqtqimw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/ghiuzcupu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gnlonifhz.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gdyxhcuzo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/geqprxufy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gpflopuup.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/guypuksev.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gzdzfoocp.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gqhwbteqe.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gtgljrxdn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gedenomej.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gfsrpihae.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gtnzvodlm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gqriinigl.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gihgvzaal.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gimpcsedz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gggstlcmm.sHtML


<!-- 参考信息 -->