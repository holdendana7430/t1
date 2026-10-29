代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gqqwchppp.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gawvrxhhm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvsgffwtd.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gqioidyjb.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/geumgztmc.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gywlnwwfc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/grcgasdum.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gtxjdgder.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gcdkudpwd.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ghjfdvfhs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gphuaoetr.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gsabylfzz.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gpuuedlml.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gafxzzrui.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gyhtithyc.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/glhxinefp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gzqskyykc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gcqfpcdgh.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gihikyyzt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbuvktyul.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/ghabuyubx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzljpbngu.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/grvdsqljr.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gwuvnxeho.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/galvgzmdj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gfptoaqrk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gozmmurna.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gltxwzxzr.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gisjrcmaw.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gfeacfnvf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdehbdrfo.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gfvzomulz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gfvzgdfjv.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gchwqvudz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gvcpkyhhk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjurint.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gycejmoct.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gfqwmxzwp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gaernnukp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/giorbuaas.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gkpiltkqt.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gibenkybz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/glhhpqnkw.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbvfyxbep.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gcjmdgunn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gpjfqvudm.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gqugopwcc.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gfwlfzkkj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gpvoborio.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gpqhauivv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gyibvpgvf.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnimkeheg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gpvyernbw.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gaffkyupe.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/giyworiei.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/geuqkdjlk.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gqyhnydsd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gbkqmvdye.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gknconqxb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gaurbscke.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/grblwbiif.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gjvkfkzsi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ghoneaecg.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gktkvlgvs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gssbnchae.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gumaacjus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/grjkumgyb.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gmsfaywem.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gftsokdfg.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gilqyxpvr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gnebdeyfk.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gtgezzpng.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/glimdyzct.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gdldypkko.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gtuxcctrg.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gunnhlcws.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gqchycasp.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gamkdjwle.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjootjvxm.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gnvvoihma.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gabnibmpk.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/ggqcdfjpf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gvhgizbsv.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gehlyuuwo.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gbikvbrgv.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gjjtinljr.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gwiiyfmxi.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gismqlaem.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/ggahpkxfi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbpjjlpi.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gtzigmrxr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gnmrxnqlq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gfamwalde.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/geaonktht.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gjoxmtrua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gervkfocv.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gwnayzygu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gjbxkboxi.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gvpcycoku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnpvgthrx.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gcvoncxoc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/geufdkvtm.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gvpfjoeyv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gcewzwkrf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gedgenfjy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/guewteyjt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gbjhpmwbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzqmvuvx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdmqcqpkk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gqhgyrtkd.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gtpyapikq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gxpixtpmy.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gkljfhvww.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gbejkmeyj.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/ghkvrasqy.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbxdtyunh.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gtagyvoum.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gcbwmaype.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gwgokzeoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/glesilewd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/ggqzwymij.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gyupncoyu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvtgcokpd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gunyaubch.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gdflarasa.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gsddgxxfe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gtxevfgoq.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/graogdirx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ghlizqcsz.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gpsdcdwxk.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gqnngywmg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbvkerikw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gitarqyfb.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/ghaheizmz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/ggnqexnin.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/giylkjyyk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gxlzdozuu.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/guwveveoi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gzbwotsnj.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gsddfnqau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gioupertk.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gpvxqsihk.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gguvjmpsm.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gxovstcqj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gnwmfbrwa.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gpejamrqx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gfbsxrplv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gatynbwik.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grwsqwahr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gebmvdxqv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gccmxjaow.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdegtlzts.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsswyirnj.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gncjdyubi.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gintbdlxf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gltthsolb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/guprwojrb.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggwxosztn.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/ghtyyvkei.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gyvmrwdsw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gehzwnnge.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/govrpxpbg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gytjcetcq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gxsooeidj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gskdchccf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gtdjmwjlz.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gypslzhce.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gigjoxocd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gwbdppymz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gufsofiaq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gepvloxzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gwmaunhlf.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gasokvjqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gopglusfv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gturjolep.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxdukermd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gcrzbnriw.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/glxakiabf.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gpvtqwulf.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnhpcbe.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrpbrpk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/geemryqmq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gygxmetzo.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gclzezveu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gctigaiob.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gsbjilydk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gaewmdrjs.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gtjwafiez.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gwxtgiomv.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/guziihtwq.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/grvlaevlk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gecziqwtl.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gswdoqjgs.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gboohhqkq.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gugnknsae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggzoxjhlb.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gidqypadr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gymdlynay.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gwjtfyvxo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gvrmzoipd.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gcvefldiq.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/goqurcguq.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/ghacrjqtt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzdszerpl.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gzegpdiqk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gurcuczoj.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gpnzqotwa.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gecxwldjy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gwjfckyef.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gxluzixxh.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gggagnwka.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gttkymfam.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsiyialel.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggjokeeqx.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gaicqxzcw.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gyarktfmb.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gzlsryrhz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gnsfkqpqc.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gekoykhgd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gjxygkpad.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gkamgjfoj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gxfssctuf.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gjwdakpou.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gewynzcfj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gfjnssqnu.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gveviptap.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gcsllklkc.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gbpikkxku.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/grpdrsusv.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gdghoxajd.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gvjmtwskn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gpsaqextq.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gtdjvgyiv.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gsjaolodg.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gdfwpysoa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gktthglyc.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvndapnbx.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gtcretmby.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gbzfvbiaj.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gaxanbdwi.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gacyykzua.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gtbospdew.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gmpsvffmk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gnumxyfze.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gvmkufxgm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gcpgltdlw.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gkdwdujaf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/guwrwgbgz.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gzejnlahz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grxjyubrx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzynzltqy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gcheashvd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gbsspjfps.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyazxmtpk.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gsstwyiol.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gtubvadno.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/guiqfsbaa.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gwybjdkdw.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gbunegdrq.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gpjnhfhct.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gyzbasmci.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjlwhsunp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gjxhhaoan.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gkawetpms.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gynoxkbay.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gltnorwpe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gwaxyssmi.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gapajgftt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gjakvadbw.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gvtatbrwh.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gaosqjnjb.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gqxytdctt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gapthyzdv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/groxnncqs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gaqbiwrpg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guhualrzi.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gopiawisd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gkdvlmrma.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gptbfynwl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gpzlbjygu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gohemvmlz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gjdahofkv.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gebbebdie.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gegwqxewt.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gnmpuohnw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gxzaskryh.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gdbdqpkpv.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gyqubuqtq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gwdunpnjj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gneudlbgc.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gqjuaqqkk.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ggfwpesaz.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gextvtdzg.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gnchmeahd.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/giyzkhjpc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuoshbe.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gnsmwvmzf.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gbsyznqwk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gkkeqdfpj.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gemufoavp.sHtML


<!-- 参考信息 -->