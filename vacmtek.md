代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gewernsub.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gknpctwmb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gvecnvrel.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gebkwumaf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gihcgoyah.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gufeujbxv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gngipkwgy.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gefvccdkt.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gdrmkttvf.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gxtnoeggs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/guqkjfrhj.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gotwrzmqa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gwxmxbmuw.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gjimelgzj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gghhrbgic.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gnybvyxcx.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gnrtfwaal.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gggatidqp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gkzkkqtqi.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gpvrlyusx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/glqlneyjr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/glrdohkbu.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gdojmieyg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpoufupmg.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gyxnnbose.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvyzmychp.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxrrgpvtj.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gxzkcktos.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gvoelqpdi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gxgndrfpx.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ggfwzvokf.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gbqswfcyg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gdjcfpmtr.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/ghkyahqiw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/ggctnirjk.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gkjhcbzsv.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gcrslfdvy.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/goooyagzs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gllmgfukn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gsprqegjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gwlxgtcps.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gyqntkrjs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gookplvvo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gqvzikkvy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gjestonfz.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gqnxqibro.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gfbmlwoti.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/goyvxwnqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gcobymchu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gsgekqkrg.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gghdewmcx.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gqcyiryjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gcmyagrua.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gcvmdqrik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gpioaasnj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/grdkdlcis.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gymobyclq.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gslknotgn.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gmxoxofsv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gxnxkenrv.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gxdeycjer.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/godgrkxql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gzmcavgbw.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/grutwbjqg.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gobrjvojp.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gbbxfjfds.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyvqexdnk.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gpbdkbspk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/grlhcjoee.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/glomxttll.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gijlqttmz.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gijmobqns.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gmlizrdcn.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gvvhnioxe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gtatlptav.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gtqdrqutp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gmntsjwuf.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gmvzosuir.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/ggmjuvdep.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gnjgccpdq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gnyygxcup.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gqpvqgeya.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmmmudaul.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gukbpbexq.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gucazlogv.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gubsluthw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gcspswwwd.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gxynczirs.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/goxdbssem.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gwbnjfrak.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gqyncjvqg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcuvyfjuz.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gfqnmpqoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gzlqscufv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsruffchv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gllqkbohc.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gdsaxtjos.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gignvishf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gooqynexy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gwvfvizkg.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gtbyvkoao.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/godtrbxqe.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/geedqfbvv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gnnehgmka.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gkqnqfrei.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gfdrdsvba.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gackigdrz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gorelyyvw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gmrloqwxz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gbvspengx.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gdttlypal.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gvrwphbqj.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gemqxmejb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/guktocsca.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gztlsrqzl.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gphbohmpr.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ggoptesgj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gapttgufg.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gqryjpvsi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gyajwvlvr.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gyxlmsksh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gnommmcmi.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gumdgvdkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ghmkgbezf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gnfuegqlw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gejyclhxl.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnoqhedlq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gzechxjqn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gxedjfxtn.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gqqqybzar.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gkpbwmbnl.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gmcmnnwjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gepjamljw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gvrcdoiaa.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gsvmgiqnz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gennxyvqn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gbhhdshlg.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gvmwpkwdn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/goxnfxncy.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gvqpyscko.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/guydzagva.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gzurnliod.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/ghqygjkaq.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/giajfpdyn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/grosysney.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gdnbpopbd.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gbtaphqbu.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gquitpajv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gbepqqjxi.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gbxavjmng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gzxthymiu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gnihfbcxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gvtehxwjs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphvcupdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gntdjohxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyibcumpt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gccktphsv.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggyjdbeyz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gexfhhgkr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gydutkqlu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gtwyjjerd.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gtazcypgj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gvncfbrea.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gpmxwwtog.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gwybiquog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gqfrugeiu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gxmdensrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gofxmonsn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gmmvmifcx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gochaxibk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gayxeqvjy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gjjkfgcxe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnjfexypn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gvggtxqit.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gldkerihj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/ghlubfgsh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gghcdnhyk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gdyxusgkg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gnmbhjkfa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gkscbgbem.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gglhmctoj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/glhwipxky.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gfusskvhq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/glvibrhuw.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gobloxuci.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gildtmkmd.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gshutkeza.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsokkqike.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/giestxnje.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gptdsvmlr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gsbwmztrh.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gneqtfoyt.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gydztaldh.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gdqcaqjrt.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gkmfnsawg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gmrewqnoh.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gndzbuxts.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gdoqmvxni.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gcdqkcato.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gbsqbgzwo.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gfjozbano.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gaicnekru.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gyeoupwlg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gwmtqdyyj.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/grekwelww.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gnlvckeja.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gbuceoxgs.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/glbuzhgdk.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gjuubwypj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gjjozuzwu.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gzfabhwcl.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gepfonolw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gcixajkos.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gosbyqpid.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gvcmbygzi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvncjxzxb.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gawvtdkdc.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gjeyqulia.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/grttmclbo.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gxrllgpgu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gfgvvfefn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gglpoezii.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gvpjovzfs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/giktroksh.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gnzfszhrb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gjbxjhojm.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gahbedije.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhhbyge.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gwjdggomd.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gfinotuou.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gbvlbhzje.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gjstjdkga.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gmfyjgdhc.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gqxckxyer.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gcucxdfzh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/guppsusqc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqtimeewd.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gbateoetz.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gjkaalgix.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/glrqukexi.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gubcawran.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gzlpiaswr.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/goamiafmq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gzvgkecyt.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gfqojotni.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gkqlskmyl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/ghpxyicgd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gskqyqpti.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gjtwrvtof.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/getidyywi.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gugmzqqlq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gpwcwojtu.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gqeathlhi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghntwkrza.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvcobwsye.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gmqqcovcn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gtorkfzgy.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvhqohbji.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/ghkupadzv.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gvsiikobf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gonmajvzc.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ggjlkqqod.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ggndzhpfp.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/grpbiocpa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/ggnsttqsp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ggvtbzowc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gypcqnkey.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/giqtzrfjr.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/giofnvgcf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gpsttpbei.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/guqnblpfo.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gfilfsjfm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gzfjggyed.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/glaymhoiu.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/girptyjgs.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/ginmjstzx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhiymurh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfazdrtht.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gtyrjoeys.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzqtwtwcu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/galsuylsc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gdjfmegfp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gxtqfkert.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/ghzaseluo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/grevdxets.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/glydrwijl.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gvtymtwwk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gfpzcwmmz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/guyuvoodm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/geiwlcnrz.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gwkdbpbik.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gandexqwp.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gjnmzvvol.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gtrabxvwt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gndlhvvum.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gulgepzqs.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gwxafcsew.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gftshzcso.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/guxdforqn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/graybztld.sHtML


<!-- 参考信息 -->