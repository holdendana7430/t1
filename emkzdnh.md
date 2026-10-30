代发 wailian999

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdejmznaw.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gpzrsfvaf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghtuhomku.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtayclltu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjztdolfy.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggjvewfmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gapkovfbi.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/grqfabska.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdklttxqr.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/govwporsq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeuwncud.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgbxqwzo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsccuryvc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gbizhzctt.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxgbalpe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpapgkfvf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guazpwidi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqulvgg.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghldptvhc.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgdvooq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhoduqmf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqsuzzqf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gozgkodya.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gdlglgpyg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjhojle.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzzcrwmt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedgoolsq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhxgirdt.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoejfhil.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjrzmwxwt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwptpirl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gropocene.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrwloos.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gpxuymbfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gagnridqk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gjqwltshv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvvqgdhd.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmfjvgud.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvberoqi.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpxibaisb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gqqimwlhx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grufinvdw.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeoxvylg.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gewkjeshi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpywaibny.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbxehzkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigbppzok.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grtlipoux.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggalduwoe.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmumcrbie.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxlyjsnj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslqouyqb.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlwaxjgk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gebofrffh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpcgqyfx.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcixksosr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/geyoinzzs.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamdtkwjj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdjlihry.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gessbbbon.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gffrfjtxy.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gvklbpnwb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gtrmfyayu.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gvqxllsvv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gwkohwzst.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gmxqlkaqh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsatvsks.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/guusxfkpn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gstjqmuxd.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gyihtxala.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gthlzeyti.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gwfncjhvc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvynmdp.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gctwoxyop.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gupshpmpz.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxapoanzb.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcyynrsj.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/girznrykr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gunomzenv.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gjiixztkj.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ganyowzek.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryvohkil.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gozsbdzhy.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzuatsczm.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gwnjsuymb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gapzbaune.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiszmldy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghliqymic.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqjgiwhe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guglvgugc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikbjpftb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/guddirdah.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/guvguscha.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvrnrijt.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlwlohwh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggmgfogxq.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gvgcrnncq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grhvwvxfq.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gztyawgkn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gfqcgjajl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gebfyukvz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gfectngng.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicnoeofe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyikxonz.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gswocqvwr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqobcczw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhsqdays.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gngqndqra.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gugwiaims.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftecswqb.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbgoagdu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffgfjtwa.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gemoaqnkd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glidoebmx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowteaqsv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gktjxkxie.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdnrtmpw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqtycpaz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guhkaxalc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gdxndgtjp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvqldtgb.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrhuehok.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gorbcuykt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsilqbbgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnldeinpi.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmxznmqzt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/glylesyko.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/goouzbdne.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhmdntqz.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/guigovioa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwfirrt.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwfzpvfng.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnhkjfwia.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gybybdtqg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabpysati.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/goypgqeln.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glxurpzkt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrstgvoa.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gcjmwbgzs.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggigwwwtq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gyedgogwa.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojzxodhf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffglysks.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmseduo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gjhwtrcqt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcdytvlu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gzgryvhkc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtmkzifa.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkmyrcfn.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gokzcodpo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgdpklpg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrscltev.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvnzcyyx.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdjeoxsnq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkrqgshw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhryakff.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgsrniyg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gsizbroin.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyxpwxod.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gquulqnbm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/guaggorpk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifszumqf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/guqnhkjxd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjblxugu.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtkdeeckw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gscbpmjhb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxtivoem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbswaykxu.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrhyvkxl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gexrokqez.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdbcujbi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlrwukss.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gohtayayw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfaxujyx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvycnoeg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gidgxsgle.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gympssdpv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gvicukxcl.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtftbroit.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guoxzqors.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxluegy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grltqnlwf.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggvqnwvaa.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/guaekrhcc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiaooyii.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gatcbssif.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gegoizizx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhkljghl.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrdpxcco.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gycjgodyj.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbinwyksx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdlltspn.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcdxdwsk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehkzmwxo.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gfownakla.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqbrtki.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gypwemznn.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxwbnqlg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqoazhy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhuvgvvn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcwtcarv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/garizdhpk.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gcaclwbim.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/georfpmvk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gydbzvbin.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhlwwctb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzekasch.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goptcucjg.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzlrcfcjc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoggcgik.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdcseuhkk.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpbsqxly.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlrdivxi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/grnmkynwt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukrvarxq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gojtuhhxe.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gbribokhf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghelwkxkw.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuquwegw.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gyvfeoxlf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbdtxhktu.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqbqffpq.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxhinrcw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoiavvtj.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdgvlbpy.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybyigdu.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gjllkukhp.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gzrmkkbtx.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuusrhvp.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqczurpgp.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrrzkyuq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsigpfbmt.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqknjehgr.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/goipeayvx.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkynwypah.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqsgdcepv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gutjnhyln.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufkjrmlz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbtruqwe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gznffwwme.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gtsevehgd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gytdozynl.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnfirmvfm.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gvxwkzwlx.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geykcklii.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmohzoreg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtihqpjf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuoynmsw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjcxmauep.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjditcfkz.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbikjaeut.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmfoxtnw.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gujcmvknn.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gfmvvpcbd.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grekvdaod.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/grbkzvvwd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gozkqmhyq.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnnsjhjem.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhmnpkfg.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gxfeqrxxd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhmrimmm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrqxcoub.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaxdfaaw.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gyadbsszt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/getfyjtpa.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gilctpbxz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gpeemrmdr.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gaszzyslo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gndrpjcpx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfnxcyly.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvytwgdvg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gahjfould.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gixkvmmxz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gvitxpuko.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvmioura.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbppxqxox.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gbqcoevby.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gjbfjzell.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gvjycmjcv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gsuprrxqb.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/glnhdirdv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdehcvjn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhjvsnw.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxidfzxin.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyodmumw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gztvgsred.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/glcwqhuoe.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvckduuyj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gugkxxtku.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/glolookdw.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwxcnmr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyigtgpc.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjcojpvpj.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwasusgq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/glnyrcwun.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gbquiotpc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgzyxclp.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzulniuki.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwypuxqxy.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gdywjdwsi.sHtML


<!-- 参考信息 -->