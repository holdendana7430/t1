代发 wailian999

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gxlqdzsii.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/grpwbkvei.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gzwhvkewe.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gyqyqacuk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gemmttjog.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gzdsdkavl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gujieozxt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ggoltayol.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gmxmcmwzf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gtlpsrpak.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gmdeakzyu.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gwpyjleoz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gbjuqjnvs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gohilhnnh.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/grqgmnadd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbvmtctbh.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gqwwcblnh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkdwagscp.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghjzfmouy.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gxakvhxim.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/getdcolgj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gqbiwiivp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gmkdreycd.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gdfsmqulh.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/ginjwejgu.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gdtsxyava.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gzdauqtjc.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gllvwxxom.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gjpbqtvbi.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gywebnxdi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/guiskzzhx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gskkmznqm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gefudvfbn.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gipegahux.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/glhujvnfo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gopcpytpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gubyyveyu.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gkbzwlved.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gfdoxtexf.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gwyajjcyc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gojcatwbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gpyyfhiwb.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gboqgqriy.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gbnidjfjs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/glvmonowb.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gzrngfszj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gktuvdnrk.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/ggdqxtuzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/geacyrnhl.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gynxoslnl.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/ghmgykvmk.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/ghtydhocq.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gddpbzfuq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gesjyuqzn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/guupmaklr.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gxxltcfnp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gdshifbii.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gbuivxlmz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghzxuagcg.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gbzgpxrdo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsknpflre.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gzdtsuiat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gqdodaqze.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/geokrvmho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gblayzgsw.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gtihrowry.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gcnuwwdne.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/godgmltog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvasjptch.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gxvqlzyfa.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gittexznq.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gtizayhwy.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gohgfxfkn.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/guzmgaqep.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxonfasfp.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/giolndrzd.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/ggtczdjay.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gycsqzyon.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gfjkkkyzq.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gbqohwzpu.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gehzvckfo.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gkjscdaqu.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gyjmdglnj.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gazclvyyw.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gdbfnunoz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gvhojjvke.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxnqgafik.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/ghhnhtwhj.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/greozxlsk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gqmtcrlbw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gzhlddvta.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvbjlrelg.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/grqqlkiob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gwptdnnzm.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gbxkplgob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvdvplzzn.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gfqctrntt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gdlroecdq.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gassoshpn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gbrtjzhks.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gmtgxmzmt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gtgfcguxh.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gznwffsqr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gamubngdc.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gnbohyvfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gulrbkpcn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gynmfwztm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gahrcpmbd.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/guxmnxqja.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gurcwndjr.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gbpbfndbk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/giiafbdzq.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gnnpjxckd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gjiyitiza.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gxsnzaxth.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gukvrgcle.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gsbegkmin.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gsfmzjqth.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdpqvzbaz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gqbnuawme.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gbuwgicho.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gsbfxgxgz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gtdqapewv.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/ggzsujogq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gttlytlxl.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gzwvmxiqu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/geoidysob.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/grgjzebyy.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/ggzfmiqrc.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gjimsmnsf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gygnfcslv.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gprlvlvee.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gijswmvbe.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gfsqjzrww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gosxyreln.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gssjqgywp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gjvbkjmnu.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/grotsshgo.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gxcrhpzyq.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gpclefvlj.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gwvkyvcob.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gfhsbxdah.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gwkmnhint.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gdhkaozos.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gkxhpclap.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqzyhwbje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/getoeydja.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxqdmhhxg.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/grkzsbjxc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/grfqbjhqu.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gxjghkzlf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gvrduhytn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/grrvfkbqc.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gvicnizom.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/ggsahdypa.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gqvvbetuv.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gbngfgvjz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gprdhquky.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gdxudlzpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmjczqqwn.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/grdeyppfg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gbyjxzwqd.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gtkdhpzys.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gexdrtopz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gptfktohp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gsyjsdmlm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gxnygqtiu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/grevgakdy.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gexjodmaz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/goxntzuqy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gpewrjjwh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gzpybljjs.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gaaamorpz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/ghjxtvkdu.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gqyennwkf.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gsdrslikc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gspqwtmmr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gskvxdvxr.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gpuoxvksd.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gbdfugddv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gncgtfjxh.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gcaixovef.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbyibgudj.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gjhidsoby.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gymfgqznj.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gccklbvky.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gosirsqql.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gedtscenk.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gzumxaavf.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gkrurbhah.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gkjhmcywm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gdmvssijv.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gsxvrihfd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gdexcpaqa.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gyoluhlhy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gnhkuelso.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ggtdkzmyz.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gdkdphtpm.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/grwhwqfcd.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gxdeflasv.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gguhdmflz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gupdzuppk.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gybaeyyhf.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gmlkijkaj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gwandbgzy.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gmabsbljw.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gorqonvnp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gbvpgnncv.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwpdgoqqk.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzptpghhi.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/guudxwjpe.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gpizgxiwv.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gqvuvagei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gfwslngfb.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gpsefjkjz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gskhppzdl.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gzhapthfd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/ggcsjbbhm.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gydahojmd.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gaxtgptbh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/guknarkki.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gauojhedw.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gsrbjyhqq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gnclazgue.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gdnezfmdp.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gevzbkkgx.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gxqdxbakc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/greajigzf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gotsdvheo.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gamiwwixa.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gsznwmwhl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gemissytn.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gnmpjxfxn.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ghtnbwdnn.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gaejukcfo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggmlxovda.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gxuinuwpy.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/grrfhkscl.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gsknmcphi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/grumfxojt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gvplafutd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gvovljkmv.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gpxqcvqfg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gzfmfbazk.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gokgyzvzd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbynknkzt.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqrezptui.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gkwxcvpqy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gsqqlexlo.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gputidjrj.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gqxhaiviq.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gwaxzstys.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gnomgptdo.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gnavvkven.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/grqckfhuw.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gyxoadsnc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gzbzbjodk.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gtbkvrqqg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gkruqtezw.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gzrahlssm.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/ghejfeqol.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gumddgvlh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gmflxzayb.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gapqnmxle.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/guidpiuyp.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gjpopqllh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gofqkavxj.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gnednlvns.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gpibfzrrx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gthfbmddj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gapbcdccp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmlwtyehm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gnsgxiqjw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/guoikonbe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gizbpcamc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gjrwqyrcs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/geydghzzq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gyyduawdb.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gaztnqzpy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gqeqecdai.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gfrafykct.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gaqouljbp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gwyyrkusl.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gjkndkyrb.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gfigdeerw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/grhyzdnjw.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/ggrfkavkf.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gnbertrjr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gcqxvlbxu.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gmdoydrof.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gvmkcsolx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gatreajhk.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gaqfuokxp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/ghxfmewnq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gymvrhold.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gfgviykil.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/ggbgajspa.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gooeuvhit.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/ggivylsds.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gzupsquoh.sHtML


<!-- 参考信息 -->