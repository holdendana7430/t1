代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghldohtzr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuturaqx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/guvqjrljo.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfxbzqqg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtjymcdu.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/giunyrdfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guyvrvhqd.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glnenewht.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gtumbywab.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyjgkkkhp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgzyqvhu.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gkrnyiped.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuttvpjg.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grelxtbmd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtljimuyx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlqxwakh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqockgx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfuyxkuk.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gxqczetbq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvuiihiqb.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzmblsyb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjcaqvjs.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtwstysxa.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjabqzvsd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gabhofdes.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnibbeuzq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnpefcmy.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbbhkofv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrcuhsne.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gyorzuhus.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctsfskgh.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnrphcqy.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqfevkkns.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gultpagjy.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gkdiduqgt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwrhchuq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gyqeiefdo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/grhancjol.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslgicwkv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gidrfpspa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gzoympucl.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gvudxrpyg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gejumckxz.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpgkjcdyr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gnurddxbz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbnhegye.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gjxocisdy.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzckozauu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvfsqvzyo.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruvfonml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/guoltbpzb.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzzptosk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gekdpbecr.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcayqasyr.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxommkniy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfnxsyhk.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gguktwinl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gddnzipew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqcdnnbz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogochqct.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gqtzsimdw.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbrhzxner.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gryvdtzsr.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqcuaeuia.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ghkpkgvnm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiupeutu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/galieazpc.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gsbsxzpid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkbhdou.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjqysdp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/grjtmqydi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrwdqodk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/giemsetgj.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gnrmskknc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqjzsjgo.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gqvmrhtos.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuyrhyhn.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvcodedw.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gxstkqapl.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcypvofsz.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbrviiol.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gztrtuxas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/glrtbjopq.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gkhefqcnz.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfckwela.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/ghedvfdic.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygqrtkkw.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvtdiarix.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gpjpzikfn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gesbhriyy.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsrrjprol.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/glfiipxjm.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuvnxktl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gyyjfzqbv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogfajnhb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumixfgot.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/glwslddwn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guhbpqvya.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gztifgusp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gierjdbnt.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayvkhknk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlxcbvrb.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnjluxoz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gevoxkfzp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gayomuzst.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmpkiynk.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaosexzl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbshvjfre.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtciwmlpb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbodoecda.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvzhygt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbehdwwh.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxqtvbv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbkrntbq.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gsksfqtdc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gddnkvkow.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gionovugr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gquqzhpbr.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gthdsiqkh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhcdyzfp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnsygxwtk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmwgmyxh.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gixwihbvo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gronznhld.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gjsbiguxd.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gffccqccv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/guwfuhjmh.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmkyaydcb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/girpisazl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gioarzgjv.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gxyotnfhs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkynfymvm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gctdhqwoi.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gccgrenlm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyauhguxr.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/geqguxztb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gicmaeqfg.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gvhabmqzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsxyjebd.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrqzzwzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gimdysuxl.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/ggggmcolx.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxraunauv.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktmgoxti.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiywyctd.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/goxqyopaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gqglrbwhk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbzblelmi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzuojdnq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gytcpunfm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvqcwcwl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkxgazick.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxlngpjny.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdweszmd.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlwnonap.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/goilmkmav.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnnpcdfu.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gybqwkvvj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigguydtr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyzwmfzd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcejjdmjq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcylyugi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsurvnnrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/govzfydhe.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gcyrebjgd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/goyjhfdwl.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gsscjfbdm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/godinqdfv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gouasjxxt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijyadsmd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzoqksmyf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gurqprmwt.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gwutnfmey.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gyufxyxoz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgbiwfhd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwxqypol.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdbaendx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmequawo.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/guxckwkao.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllcqszag.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gmmooijtp.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/glaeobqxe.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnfirommw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoygcnch.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggavaerri.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvcskkqt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gftheuqjr.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gdursmntv.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ghypqtzci.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gztcydmaf.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gchxlfdmn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltdbqilt.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/glskdclww.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrbmapgq.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grwqdcovy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxbogabjp.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggacrmapy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gthijfccx.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gmizqnlsy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxxyjubtf.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gebhsugzc.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/glosyvchu.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gazvmxemg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyecgnqc.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gstzxcwzi.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzdzxawow.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmuikiegl.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gqrefqyhz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gwypzpazg.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/guhelqhaf.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gimvdrvcd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqovkktb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grduzxnyh.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwsmbmjn.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghenjaine.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gbmyekvgo.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxriehmx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/geunjwzwh.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbrsgwcr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjybjklfh.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgxcyxy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gdlymayst.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gifkhracl.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvcelvbk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gyuzxvxzd.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gratrytvg.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgcfqava.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcrrmvsy.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkhnxam.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gliobxakp.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/guafttnru.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghufcmthx.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxwkdqobk.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gafnvaqpt.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gthdefuox.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtfsdouz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzpplwtx.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeufmlgd.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbywrms.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihrcedzz.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjjnotcyo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpylskoga.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gberhwhnk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gobxnaxon.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/ggisrsszk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsivesuyd.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmzzspjk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/grglhgwrf.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrdiuxsv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlqgadiq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwpfcyrdg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhqjufzp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwntazfoc.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guvohcmvh.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkvdsxxq.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geqshjsql.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhmuaoz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdunprvdb.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpshkiihy.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjoarqa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlxvjfor.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjytigeon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhptikig.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gyqixjjyv.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/guwwcgtot.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfqlmyao.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gcyhfckcy.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gtisspobp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gomobgeca.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvpicmogt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwujlbyq.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/guqxfaytb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gejullrfi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkgwchgy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfljicyhn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpbsuikno.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/geehxsyin.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkebdfedi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gfjjyaekt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzifcgvbu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqlbkram.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gmeoaftug.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gbexlxzck.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gptwepuxy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvxfytqr.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvgteyzu.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gzaoekxlr.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgeojhtn.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaezfsse.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdwbpnub.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwaddghi.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gckhxucwn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujzmetkz.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gqahtlwtr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvcuyaki.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxvvxrko.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjlivdsl.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxauuucfd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gstqcbgwk.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbzhahfi.sHtML


<!-- 参考信息 -->