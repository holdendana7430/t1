代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghnmvhmh.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgojyrtw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gzhxgevyd.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgfaphvq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdwchtoi.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/givtqkdqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdzckecbg.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqpybwdjp.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gucdcgfmc.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskcikflz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmnrrswka.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbjravyd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/guestrfvn.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwfhzuuzt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpgbcvvw.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/guiwsnkew.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsetoxft.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gpcfcusox.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gilxqiqpq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gynmfonan.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gywposums.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gwdfjbyxu.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/giwulyhjm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwkvuihs.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/goasjdvkz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grytfoahz.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grsdefdfr.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/githqqdbi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmacizui.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbanoeky.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/geynolbod.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gtxxpvjby.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/grdpzfdlb.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvddpjlaa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfvizflt.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqxhlvqm.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhkpajph.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gogxihfrv.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/grejkdpjq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqicozys.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzxlgku.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gyutmnvzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gqkxnolha.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guddlbwue.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/ggvtdddcr.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeyyqnef.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtbjktch.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyakenbgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmmybkus.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkdwxlay.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gpeyfwqhb.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnsvrfgv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvptngtal.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gyjnlcdpq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsnrhopd.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaolgjbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gqcdnqfad.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvleayjfc.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnrjxlgn.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gizqpgnbf.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/goewgmfhk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqqnxejy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqqezdvs.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjfonqwp.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/glfuokoro.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbmtgldh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfurvcapg.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuwaoqpp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gukvxbmef.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gqyguiuio.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gactwjfqk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdvwbeips.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gzabbarrl.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gxuwwjzzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gophpjssz.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gvgiikfhj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gbdfcqufn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtskcnkw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmouaknwq.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtxeosar.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkozlghm.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grnsasjra.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gntllolic.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grmchojje.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgamekyn.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guykwzttf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gwbvijxyw.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gymxdmdqc.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlarbqev.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/giexpxoqh.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gixztudeq.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gapsyzhay.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddczrowa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gendgqdxk.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjghywiy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzybtcknu.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gbfpszgjp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnpecvwb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gxllzztol.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjikqlnz.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gfxswggof.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyazjujy.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/goszizrez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgaobljl.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvrvpknc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoqvqrla.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/garttqnym.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/grdoevzgl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlwbdzbt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gnkthxmdf.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdotwkafa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpqcyhykg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gayqepjji.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjgrlaqyk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpgtvsehi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdekkrjjf.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/grbiwwjuu.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gqheefeor.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gmxiuuamo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqoyzzsy.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/grpjsznyt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglflfkuk.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gopbqauje.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaadstxgx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnrkdsdxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoefesya.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvurnclzr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnnlwtnt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmpccian.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoygdvmo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgoiejzg.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gomvqgote.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gsticbvzb.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guewspems.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/guypdfoyt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkwtflel.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybkcpsbi.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjxcatcc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojfpakm.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gbssbhpce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/girmrkptq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gvoptdtyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbdrjblng.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrktvdwj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyyjqepu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbfyyhin.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/goyqmkfsz.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqnclqpf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjyvotwnu.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gvewlddrc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gljtyyznd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gswdkqnpw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gcltiosvn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbuzlwwsh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gqlyzhwsq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmbzvkmau.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gueldxobg.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkndfxidk.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnasuxru.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbdzzkcm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqdgrver.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjorntfh.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gkblyrota.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqndjcqrg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gernxyuga.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gmwgumiyp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcmfvosw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpnxyody.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gispmyary.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkqqvlrxt.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdcygbtp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gfwgebxzh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/grxfbxifl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gykzaywdb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/guywtrtkm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gkhurmldh.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrvmgowh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gejxizuuw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnjmfyme.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbzuktgw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpydsdid.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjhtsshe.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbciiybx.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gpookmjxa.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gcifyvzqr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/ggjgrwksp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govrhqoxh.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvlinvwb.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbljbnun.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkwxpnfd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyylgxdv.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gdijtrbze.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/grfvnantl.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/glkoblzus.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gfysmxskd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmilewk.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gynmsaajl.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmjuaxlsz.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gqgyczikf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkljblfzz.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmbhiqykh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbisdmthn.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gyadmyhjk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhzgflhi.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gxddexjtb.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gwuczlzwd.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/grgbypvpx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokmrrtlw.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glymocmyz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafkazyda.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzulamon.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwwnjneg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/goyvzfbkb.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/grnzhdjwz.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpbiduyn.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gasvgaayf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwkpchb.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyeuhhcq.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqlbscgnk.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuuwunnf.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/goftzxktm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gtwmpukin.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gngovlcbp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gkamjqzoa.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gpphuoxyi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqwyaciin.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrxcjlcg.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gelibxdvy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gafkdflqr.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gxokggqyq.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsucbsje.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gyomuekwz.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gzsmnrxzt.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvwowwcn.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gazahhnir.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwxorswg.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghknfvsew.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gojqsblug.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gkptzpnhm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gethiomzt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfqxxpnm.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gbevalmnu.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gruyvxnis.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvczvgsta.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcbqiykgl.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxifcsyx.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gduqkfawr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhrpzzgp.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeyvgdwi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfepjvteb.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvwbvanvu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizmjusxu.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gflrqdntn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnblgjton.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glitlxatm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gbpgwbuog.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtojvzyjd.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gufwwtbap.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpmvbfss.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnytwqodn.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghwovniex.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdlkemysa.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckgtxxbq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glurqjwme.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/giqvhsoqg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmilwtu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcipcqpb.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gxuqjajtd.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/geduoznys.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gijkvkxte.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gnefxflgj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gitsvlrlb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddjbobrt.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluqbwpkw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhekoavo.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkztmsil.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkmomanb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gexxidtur.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkabgovga.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/getlvqsyy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbbpxpn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gbcuwtjye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gjetikzmo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmderfqa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqpcmnx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/grxforsgn.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofolrzxh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbhfqifp.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gjuknspxm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/goizdirdk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqkkwnwg.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwewwsrp.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gfvoysraa.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfvwjrqe.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/grbooqsmo.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcevogqo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxuwdisu.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gszguoaep.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujuxrnyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gyxmikseo.sHtML


<!-- 参考信息 -->