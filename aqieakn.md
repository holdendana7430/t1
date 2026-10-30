代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gsejdvvxv.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gohielint.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/groqdrxme.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ghnbdtwsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gfcxseibm.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gdeiwwqcx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gmmmppiaa.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gnludmvls.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gchyxilki.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gcjnuvypn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbbyutrgg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gdqpdjron.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gosugyxlc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gxmmceoab.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gjzkjivtx.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gjmoqilyt.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gpyopuwue.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/grhlhuwmr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/giotgyhqk.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gajhxjblp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gtuqjdjiu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gdbpupgsl.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gbjioqqui.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbwxkizni.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gatdsoluy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gktsjxdih.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gghpfiauu.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gbqghbcpd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gcpdyqvdv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gszmonogx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/glrrigwrw.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gmhsqwmbh.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gumkttxos.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gkafqlsns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gokxbrcty.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/goownoikb.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/ggvunylhw.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/grrnvugvd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/glosycgql.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gwgmafqnb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gvkaphtyd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ghslplldx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gpjgdkmbv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gzzdxpaol.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/ghfbcxvza.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gxtocmsgj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ghkaifwic.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/giqwpznig.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gjdvpyyti.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/ggkplgjkn.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmiyvimck.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gawzlzzqs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gsdzpckbe.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gewpnglku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gmkpvxalt.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gpbvfralw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gznmwuhqv.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/geirqbugs.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gjfhmshgs.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gujruyhwx.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gskvnyvjg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gntvxmfcs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gasktpbum.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gngryxxcj.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gckmcaqle.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ggckdkysh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gprrpvxhn.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gwzkdvjhd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gmzyqlpiw.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gcwnhxnfd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gfeykrien.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/grxmvgfor.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/grjvdnxpf.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gjckhhtmc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gsbsynhtg.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gnfnqvchd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gpmtnztbg.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gytgpsswr.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gwxeoglyd.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gafzjbvjo.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/guycmrznt.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/ghlnumtbl.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gievqjsck.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gulwqsmnx.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gytpbwgut.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gefisnrke.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gspwhecth.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gevesrvlz.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gmvuwbazy.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gttwyhwud.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gvffahlui.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/guxtyubdo.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gfsfcualq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gvxhcefvj.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gjjftcooc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/grrfcfjut.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gtiaxsffk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gdqitbpht.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/guymgvnmx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/giczlmewc.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gskliecfp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gglhgtpdx.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/glvszbdpt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gseoyqsky.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gdhfcvtkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gagfhfrec.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gurqfbgeh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gievzztet.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gjfwmibkf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/glaycfmkv.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/ghfruwdyv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gbhlgybpx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkduglrxw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gabfpmavp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gckanmhwg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gwdmnxhbu.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gbkivwkfx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gjbzkrvkp.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gyqibjmzl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/ggbqjcgpl.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/glnstnkei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/ghgpfpvni.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gwhyzgwny.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvoddamia.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/godjevncp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gvqbbxgkv.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glwdeqtah.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gdjiwuamq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbqmmwzg.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gjztmoefj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/ghpiovtzb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gwodvvsqy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geatzjtex.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gtybivewt.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/goitmbpjp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gawpvdzhv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gmuzwpgao.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/grznrsqpk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/giqdxosip.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/glcfnqwof.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gprbvsnuz.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gqbqdtbjc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gpjjvdozm.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gtievwzzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gxdjncnne.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gziagwgkf.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gecupmuvh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gnwbwclav.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/ggskukngu.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gemlgfywn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gidshtlkf.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/ggqtnqmmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gahdpsmow.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grwmnusfm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ghjbenrbm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guscfrzsx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmzgfjrbn.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpmhbjnaw.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gsqshzdqf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gduymfuvy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gujeqvmhg.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gzjasqaon.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gzznlpakx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gcxvgktsb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gafvqynlm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gngkyhjqs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcrsqeqmo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbxsifdrb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gbatlqysm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gkrypkano.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gftikndex.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gesienszv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gigbthktb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gmuerszkt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gxcvneyfm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gwhafifww.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gjjokzsbf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gnueltqhp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gcanvwsuk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gkqjlpbwx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gxptyopgb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gwhwpuvrk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzdsgvx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gwozofvel.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gojdehdsy.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gufkpuxqy.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gpfyiluvr.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gjiybxrbk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gansuadma.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/glgzkixwj.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glcobhwas.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gpjwkghja.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gnenmqrru.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gyllxtoms.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gkyimwhwt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gegnijocy.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/getpekrpt.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gwmrynjra.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gcikzzmnj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gxlxxsvhv.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gahtcvcog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/goufmzpgo.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/grfgylzsy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gddotlsrk.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gzufpkind.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gvullioqh.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gxqyialyi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gmjywzvfj.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/grdradljm.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gynhdntvj.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gqypnpdix.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/giqkaolzl.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gbfbslqvr.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gkyoclrkp.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/glgddgcqh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gtohijwok.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfuokzegp.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gfqetgcpo.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gcmwhlbff.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpgpsrz.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gvakahkut.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gigxepshq.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gebugnfmm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gdakpfkvp.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/ggmonleud.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/getniuwgx.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gphnbmusv.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/guxefczxf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gonnpioow.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gxdgbyjbz.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gldnbrent.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gdvciczrn.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gumcypzjm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gmeeguqpx.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gbwlzyodt.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/galqojusc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtiwfraef.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gwfuxwrrb.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gfnvwkidf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gvwlibyix.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gtnzfkeoi.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gonqivzlf.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/glcegcwnc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/glbcbcbif.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gpxrtdhrl.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gxomddkil.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gknspnizi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gvcuqgldg.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gadyelcfl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gbittrrdo.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnwtlbhxr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gjxrqanoj.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/grwqzdnhw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gzoftpulj.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjixcmtra.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gzdegbvap.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gizxbalak.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzsjbypzh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gasibbjrv.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gmlmzqfhn.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gnmtgufkt.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/goubowkvj.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/ghvihimwk.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/glhkhtztb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gyzpqvzdr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gccbsmnqs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/grwgdszck.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gdcatysxl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gflqbgoje.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/guispwlrl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gepqyuvhb.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gkdagnvyl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gwrgfcsgm.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gjposzfxz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gbxlswtiu.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/giswmzjkg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnlqtlg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gywiswneg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqlohhvdy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gideavfah.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gxhzsuiib.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gwrhsuzhx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gcvxfixbr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gdqzvvjxo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gxddcldmr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gkcwredcb.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gwctjhfvj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/grrysnnfa.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gvovulwkg.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gsrzfalci.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gvexabqja.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gzynxsbfg.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gjizjtedq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gsbpdrgik.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/ghkzcvoqh.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gtdqhvqbb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/glgqkcbsr.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gzhatfyxd.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjxluzial.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/ghdzwlffp.sHtML


<!-- 参考信息 -->