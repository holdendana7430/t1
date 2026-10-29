代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/ghoubwiob.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gtkstywqf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/ggyfihajw.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gqckwkkun.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gcgpmuysx.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gqjexjwqy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gabykhyjb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwndeffow.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gmcumdedx.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gjcxabmre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gaoaswvvq.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gfxbkajma.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gpjmolfst.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/ggoyrawcy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gkifgbbdp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gvztiywjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gpgckgvup.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gxlilyuug.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gzfkvtmqm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggttsewhf.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ginondgrf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gljwrgzle.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/giqjdtqbv.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gwxjnyfbk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gleawbmws.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gnctnslil.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/giyjsjqhi.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gxsudzank.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/ggvmocqze.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gnrrlfzwn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/geuhnduiq.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gtoqsljaz.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gnsyqqiju.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gataadehb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gazacfwri.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gxwudmfpb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdxrgdlgd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gqucpvzil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gkzvmkwue.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gpzaotzmh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gtrgrtnmx.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/glawnannr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/grwfvlnrd.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gelehldth.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gaoddpelb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gpsrbncdd.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/grqsnekwi.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbndmffqc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gjuuwilcm.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gxigwvarr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gewwxndah.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gnrcbtfte.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gasbrbnuu.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gypitfuqf.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/guuoagyvm.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gkyblwpup.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/guiiegrzf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gpxenjpat.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gcwuarloj.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/glaevhtiv.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gnixnpdnh.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gxxstgatw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gybujgzva.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gqnbpdqtl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdjvbagjv.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gajqetrji.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gexzafqgo.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gqquwxsbl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gebceaycn.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/giglucsia.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/ghwpyvijb.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gzpidfhfs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gvgmtcztx.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gponqmiep.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/grmhxdaih.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gruaiucxl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gfowudfwa.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gmfwmgaxy.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbaqyoiih.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gvxzswvof.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gfbciqcpl.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/guyshjqjq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gahjaoplm.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gshygcqsy.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gywujowpj.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gzmnzhtee.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gxwrvjgpk.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/grkzcmwvp.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/grgxdpnni.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/genituhvw.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gpqtuname.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gbhhmjiit.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/glhbwnqbk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/guwpybpdx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gewkmmlkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gakurpajv.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gkyvjfpqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkkuzbfdo.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gnfhixchm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaxmfoxja.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gcqdbtfbc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/geqcwhuxo.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gsmgqezns.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gpwiasnqg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gbpvzqhzc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gwbtzzate.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gwcalvxcw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gvnzfhcjb.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gvlyafwhl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gkqqqpkai.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmlkaclyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gbxvmbtvt.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gtddllxej.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/glvikuwel.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gcunegcdi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gzziivhmm.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gybrxwago.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/glkqxfaqa.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gsngqtidy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gydypodxf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gfbxfyhcq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gibnheglj.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gobhecoui.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gkqugxafe.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gyxpjvmkf.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gedksbnmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gptnizsfk.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gbhrxfnxf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggesosrmm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ggeyqcfbx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbrfvxgxi.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gtroovwxc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gzwfziozm.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gmfdttebe.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gvoipoatq.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gimuazhpm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gzlxieiun.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/grjrmqldi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gtziciusn.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gpgftglxg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/girfsfntn.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/guvrwobzr.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gkdojagul.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/giptgrjxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/grkulnwrt.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gkvdjshtp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gjyqmnxeb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gvzwuziug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gxkyamdii.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnvxwdvhp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gwwxdobdw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gisxbebtz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjxaxrovm.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzzzpnsjg.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gmhdvsffo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gyyycgelv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gagcylzvj.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gimflqaak.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gxafgzrxo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gmdvmkkwk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gftmggpsh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gbzdclcto.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/grpknwrft.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gxdkfkaul.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/grkqsgukn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfihfwcoy.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gyfvoheux.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gavexvqwh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gxdvgmddf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gidgqzabg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gpamaizch.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gguhegceg.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gphzuoddy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gvgluvbpf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gdehtaaju.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gmauasqqx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/ggkwmkjbu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gvfoocfdz.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gckhogszn.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gozoptwbv.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gdafhagrn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gmhjhcpnt.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gdegjccvq.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gogukihgq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gyvivcqjs.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gvrqzxkbh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbtgahstj.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/ghwzmdavi.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gvskdxgju.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gcsqltzgg.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gdpnufgpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gzcmbgtbk.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gciabncpx.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gnnmdhdeg.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gbbtsuovw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gqjosisse.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gjbmhgjlt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gafswscpr.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/giojlhszc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gynxuhtlc.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gotkyixbb.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gukghexwa.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gabwqhcfa.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gzqnlqono.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gdlcwkcvj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gesuockni.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gfrdfcmam.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gsqpszsim.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gavggfbhv.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gxqqhymzd.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gloifrdbz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/giohtzxkh.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmcyyphbk.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gszwhcqdf.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gnqwxrwca.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/glkzyqqkd.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gldofqfpp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gfgwcuwve.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gssqvhcpx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gprliubkc.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gulyhkjnc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gavykjrhi.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/ggvmvdgsa.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gjldkayhv.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gmxnflqrc.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gclbzgknk.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gtzvaegxo.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gbgwhdtdb.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gupitrwgx.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gnufjlzrp.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gjjcmsnhm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/grjbcrnti.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gfpmcacwz.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gjxgywuto.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gndrvjdcg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ghjhofslv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gyrokapne.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gunujaahl.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gzdpmgwwy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gbgzjpkmh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/giyaegbnl.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gvgaaivol.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gxrvclqzg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gdexqcfia.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gqucpltvv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/ggjgbixvm.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gwnmdarez.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/givmnyspf.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gnffavsok.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gpysrcgsr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gmmmgeuwn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gmpmrpjcy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gskcopmkl.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/guecsvdka.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gltcaxcoy.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/ghsvkptde.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ghkvgrquw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvzqdtkao.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/govwagcse.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gorgvymkq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gpsgxnrzi.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/ggvbjokme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gyuwzgypf.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/goptqencm.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gqxalkntd.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/geicefqql.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/glajvgcgr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gavnxdpfh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/guohayzee.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gxeptimpt.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gelhlszqh.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gfeywynpd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gebprakuk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gehdebfnj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwfqvtwyi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzlveoclz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gwmwvshon.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gurnmokyv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gyluxcimd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdxscgadh.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gvaighqaz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gbdzlbacd.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gpkthyysk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/goesfksdf.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gmzkatmhe.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gjbktbhcm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gpujyzfwk.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gcaostssq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/grryhbmaj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gfmekadey.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gqcmakmnd.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gqkmlybfs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/goqatudjj.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gasprmyuj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gfzebbuwt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gpfarueqh.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gpivsvqdx.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gpoeorqqn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gpuaamtfz.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gwmpvglax.sHtML


<!-- 参考信息 -->