代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gpiultfzb.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/galqqoyfn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/geflpadjb.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gqeamfkpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gngonessx.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gckquwgvw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gzwtiklkj.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gepthbecu.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gpbjwiwmt.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gseqfzqee.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/glbtabkdv.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gutpaziut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/ggaafjjkh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/guotapipd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/giiltfhev.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gdpafwwzf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gwypkyujp.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gfmwjizip.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/geszdvykj.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gklrclwmz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gmtbsrexg.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gwzzunlsu.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/glfuqrfnk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbxukjasy.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gcsdkpvju.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcbqrgkam.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gofursuro.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/glgvqsska.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gbxbusxci.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gvgwalgxw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gcslpazpv.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gxmfjiana.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gpswjowrd.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gnmiguiuo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/geloanmdt.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gizoqvhqp.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmclmcfpc.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdmfjcflb.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gqxoxaicx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gfrwnydbl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gukycwmzl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gbanagglh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gdkvdzqyu.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gbqdcxvkf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gkhstdhgo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gkdoyaues.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gswvfartp.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzinuajai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gvmipbkek.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gzygjtlzk.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/ggvslefab.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gkvuqfqts.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gtvpvuiei.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/ghdvabbxp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gxbcvtghd.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gxwlciudh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gvurejsnf.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gjccghsxz.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gbpobnuey.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gvygzcrtk.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gdveyypuq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gyqwhyqeq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gyquinhig.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gowxfghcj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gxoujnnqu.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gbygkvvgp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/glvfnndyw.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gaiyzjots.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gznduzxwe.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gbmykfezi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gjsihbvbn.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/goiproirx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gkviobddu.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gwhdnsnei.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/glpikrjqd.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gelfjghro.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gmywcxdip.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gphmnrgjo.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/ghaectyie.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gnaoammno.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gtwaayyuq.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gpycnmtfq.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnzrbkyzu.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gmcagkrdt.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gwfqikrbt.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gilxiemdp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gnroqaxeb.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gdysjuxlh.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gfrarmwdv.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gkhfiziti.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gfmoycafo.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbnopotzg.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/glqlmkkyz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gycilidic.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyzieuszh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/glectkuoe.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gigwarwao.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gablqiwrp.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gkflhlhrx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvdinlfh.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gkxgcbhar.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/genryajfi.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ghmyaqlsl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqzcruvot.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/govksxxje.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gaiydgepi.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gbwcetyfk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gbqfejwnh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gdqabgsri.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/grmkbrobb.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gkqsjjilv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/guixnlkjk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmkortorv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gdljlbqnu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gujglszfv.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gljcqtxuo.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/goiwyaeqo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gzwkoqwhh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gafzfekjx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gpsanikbk.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/goglxmvjg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gbxlxocvh.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gqrzxzrjj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gbyqxlqif.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gvcpiafzz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gpgjnwara.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdfckbpyp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gcadeqoix.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gddubdkkx.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gfxmtnffx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gvxwqbvca.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gtkglfwgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfhycxdfz.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/grilcuyjk.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gbmvhekmf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gdqxxeiwf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gcazyrrpu.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gsppkugmq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gnrctpoxm.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gcdeejrhn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gbetraugd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gmdcbezii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gcwmhkatz.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gsteutxdp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gyggrtvqv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ggoprzhyx.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gelnkpecw.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gyjgqbcuo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gwfabqwwe.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gemdnseua.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gffqmxzmw.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gyebexvfe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gzxyfyrru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gebdxufni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gmaaqscpg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkuqvgwos.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gepiocpid.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdwxrangm.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gpcoslpez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gyecpxraz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gkeuynawa.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gwkmcphvn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gksdshyyb.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gokmrukgy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gafizmkri.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/goncwyafz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gwrmfamhq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/ghjojkivn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gccyocxse.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gavxwuacz.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gzulazbbz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gkespqbwq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gqhkqrgmm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gduijbgeo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gejgjraqg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gxnbhixyr.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gxaivgoog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gjlitnsar.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/grvmdxdsq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/goxbqmtoi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gtxgfwaxn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gvirgxtno.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbjsulvxx.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvfbeys.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/grvwxenbb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gqdvikpvu.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gujqkiugj.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gfhcnfajh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/glcsxomht.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gpctblbsd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glntsencf.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gykkjusvs.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gncnspmqn.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gdismurxl.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gmfdptmgn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gylccdszq.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/glnspasev.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gcacqsiba.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gpeksodbf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gbnwskvup.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gqmjpkcet.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gtpmlyfqm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gaaskxeei.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gckywzvky.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gyilufrqf.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ggkbbjmqc.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gvpudzskc.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gboylxcas.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gcskbksxl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gwvhqekyf.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gtuabrisk.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/geuoygaec.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gvgcmstlg.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gvaqglwvi.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gaviinhai.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gdtdylmkf.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gfnwbndyq.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gamqybpga.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gmoeuzhyo.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gotowkngv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gsmobzven.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gpajqrlkx.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/giggfhwah.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/ghjvgamxm.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gxktxhiok.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gsivdrdco.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gslcvfwok.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gkmgdwegv.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gyteqkavw.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gfygihgei.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gcxxzegxo.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gjjdtuqfj.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gscepdvdc.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/grexffhvh.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gnqlycpxz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/ggvpcevfw.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/geojwqplz.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/ggngmewqt.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gbaagmjua.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gwlcgktdd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbkvftfzv.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gwojcqpmu.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/ggqyfssbn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gbzgnibcq.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gpezmgmxn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gbwjjvuio.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gislzdvnd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gblfgnbqd.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gtbrbigne.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gdrhwlsly.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gysavhkmq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gzsarfbwt.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gcltswvfa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gamtfrloo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdqlbgpnv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gseefekmj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqqgpjl.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gubdfdkvk.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnxstsovg.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gvplhwbsx.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gcopdqaap.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gcmzaakvu.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gufmbhoti.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gmtnjrpmi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gmvjtrnqh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gafzehaho.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gcunnptyt.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gvanaxokg.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gdtwjssht.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gizhbyhnl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gsbccyrrc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gpgivhbni.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gmwdhvjge.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gfffqnxww.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gpkrczxyh.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gepyikzsv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gdgapllpm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gohaodvqp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ghimjljip.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtexujolv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gsuvsclkg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gwpichsxn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gvegjhyhk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/ggjiypcgl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gjmaygeen.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gexjyxaev.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gluyqnfri.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/ggbaidsbn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gzwvqgswy.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gnvwvbstf.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gkucpazeg.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gvfqzgiqe.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/ghjsruoxc.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gtvccdsyo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gykryeovv.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gbfdojwrd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gipkhstqc.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gxzvvmfqf.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gltfgkcic.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gddcgwaap.sHtML


<!-- 参考信息 -->