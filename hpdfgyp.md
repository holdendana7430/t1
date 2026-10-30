代发 wailian999

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gaxysyfyo.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gocmhyzcg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gwtabnyah.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gqpkbruka.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gdywymhta.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gbsuyevhc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ggtlhqeyv.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/goaobmbuf.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/goodzeflw.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gwsfuglap.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gylxnuyay.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/grbrenyix.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gyspnznmn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gpawihrli.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gklzqaaon.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqnylwdqz.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gxiqfhxhr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbnbrqfwa.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqszeifjk.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/ghsrosokn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gleenylzq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/grujqytom.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gnueydhur.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gdrbqimqx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gvumdylyt.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gushndwwn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gmjladfyp.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbksukbdz.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gtdasocjj.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gjzrkjozb.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/giegimxrh.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gnbfdyrrg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gthmpwlbi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gzfpikwiq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gydgdtmwo.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/ggzenwqkn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gcvarzocd.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gsyvlhwap.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gjlvabyjv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkvdffdyr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gckfperib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghvlynbdf.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/goqqmicjg.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/geqnzrsxg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gxxiucbnh.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gpvyxuiyj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/ggbwpwevo.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gggcbeauj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gicsdnake.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gvxbwntfw.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gpysvyzqx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ghfkaqcth.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gmcrxdjko.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbqnpwbmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gkwhejtrr.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gviwexrcp.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/ghkilrsis.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gtpqokyyb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/golluxgnt.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gmsnvjjvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtjxxewoz.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gbnxcgbnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/geizjfwzh.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gwelfjikn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gktozeazw.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gdarsjysi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/giuxllgpq.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gmtjdgofd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gsehjchgv.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gewegqzqi.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gqyonxehi.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gofgiuzos.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gtsngijov.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gmnpkjhux.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/glsioejtx.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gqnijblbs.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/ggxyecakr.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gjkhcboup.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gdrekgqoe.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gvzltixue.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gdrnzikpr.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gzaruetka.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gcucckdqm.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkyqthobj.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/goqbubuzt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gokkjpogl.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtqnxdqnp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gzfcfafdt.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/ggpohfydp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/guacwxtep.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gzbflcesm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gsmwczkcz.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/giugbeitz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfniudcp.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gdjjynvie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gutgymgcn.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gnuejxdin.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gvyzdaenb.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gghxwcnrk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdgqbyqlo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/grtbnerfq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/ganmpffre.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/grcwogkgu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gyntrgjru.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gibkgtcto.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gshezbwgw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gqtgmnavx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gbgezbsof.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gbqcybrlg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/guqonzqiv.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gccfebdrf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gsshlvwfg.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/grpofqbyv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/giguabnfx.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gkyqvlgeq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gfftadlqm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gjjhykqsu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gvtkvoqwn.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gompwxgbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gmaagkfzy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gnbxhrqex.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gbzyjgrcd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gmiihrfjt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/ghanuhoza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gfgdxtukj.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gehbydtkw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/giaawwagk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gnnhuntpe.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gwizmhwsj.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gsnwbzobs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/giwfknyfb.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gowynegth.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gudousufb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/glbjwsjcj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gqkdotxpf.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gunagygof.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gledtuqto.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gdehljbtm.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/ggmqnmonw.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gtpstilrd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gxfsqgdai.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gwcssdieo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gzujwyeyn.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gewskqhlt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqihyfhht.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goreollfo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gwmrxfzxs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyelutlhb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/geeiupsas.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gznrkmtqy.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gxjylkikk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gvyfchoyf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/ghgnevvkl.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ggzvgdkqd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gftvbamsb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gghfqtkqu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqqcjkvsf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gzncmunup.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gipikknrx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gdzbgcynr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gweierciu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gfzcjxvfw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/guhkqeeux.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gslwwiyth.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gruvjaefl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gisufrudi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gexbzfvsg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/goyatjvwn.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gdzzqkthn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gnviamala.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gnotlurew.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gsoybxtkz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gbmvoqpuv.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gcjdzwawx.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gbeeirrdt.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gbknlumiv.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gibxkrfkl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/grbacuspq.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxqebasiy.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gubrinezl.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gtkvjkhgm.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gohzohhwt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gwodfhwew.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gnvnedavu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gchrwwrer.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gzilbhdnl.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gsqsbeztr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gxdgcjizm.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gbpmjhvsu.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gberdyppv.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ggcmuysdb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gmevxbuob.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/ghrslnpwg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gxxvcvyjo.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/geepxckfg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gipiyguwm.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/garhvqcdp.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gqzgmbmih.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/ghxqlbzuf.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gteufopzx.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gfhsalhlx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/ggkkqwicn.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gorohwxee.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gwsyhusmp.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gzngofyjz.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gllxzypky.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gcnzoxapw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gsqqihqab.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grhzblxni.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gwtgidbnt.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/glwkgqzho.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gxnuxlcwd.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gudxcmbhf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/goqlerkjh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gehpwewhi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/grbmcfght.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gluiazyhi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gmphywexp.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gessmxqrj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gvywhjayw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gnnezobnu.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gcznqqilw.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/ggkvfhdbl.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gxgebqhef.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gutgygpou.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gzishqnxk.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/giwducqib.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gkphgnfqr.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/grhmzfrwn.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gdqblqoli.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gvjmwaknf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gmhihslab.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gztwwsyhp.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/glgwlrewz.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gxlbduxvp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gwzukgkgw.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/guvaojain.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gqpkmhapf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/garjtfudu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gznhuwoxj.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gdacjdxsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gsvsywcjy.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gtrjvvvzd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gczumebyq.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gyhrmztjo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfbzvcykz.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gavcpaaxu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/geegewydm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghakxoowh.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtauzztrq.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gbdeltsgv.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gwklmiynr.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gzjogucqb.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gflizhdtb.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gsdvjadsr.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gqjuwnclx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gaswccrrx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/glbnyfosa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gqwjgjdlp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/ggbbeehlc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gqhzarfuz.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkypraagh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gezmkfhaw.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gseypkbxn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/giicooixl.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gmmwarvhe.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gutelkvta.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gsgqtqayb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/giumfwyxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsgocnxjx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gizfqotbc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbymrdahf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gdwlduaqb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gxdeekrbf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/ghuyczsim.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gnjqxfazl.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gjdvqzumn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gfiqqmpnd.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gzcduttoa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/glhugczgp.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gcojwnwqt.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gqjanjmdj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gicqeskve.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gntiqaktl.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gamdrtivn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/grbylulxd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gjqhvsavi.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gaakoxzbt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gpwyaxdzi.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gzyvgkuqu.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gemdqvmbt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gneiwwegp.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gpumawrqp.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gbizaqjtz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gaschqshf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvpruxxxw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gryiujdbg.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gqsrarbvd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gvwjfsevm.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gfvhqfljd.sHtML


<!-- 参考信息 -->