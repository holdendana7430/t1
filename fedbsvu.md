代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gjgtojnnk.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gqqcmjcfw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/ggqcsnajq.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gyojavpse.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gsmuojttt.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gxkqfjjrv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/geeryhvdh.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gcnrtkefk.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gpzjzlret.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gazfxpdku.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gadvqsctx.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzooqnxex.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gycthrfik.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/ggusnxhee.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gprcduyre.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gbhoywlji.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gctmiaphq.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gyensuwuq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gvyiprcvy.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gbcrlazsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gethqxjdn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/ghgxyosde.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gobzovpfd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gojfnlagc.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gkrkucjei.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gweauunsy.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gagcsgiuw.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gixqkfoca.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwcvodtn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gnrqoexvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gcemkbyde.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gioalfmou.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gheukojxc.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gwnteiizv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gpmhvhwun.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/glpaukhzj.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gekzmzogh.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gbgloorjo.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gqxceiskd.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gcxrhqvms.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gxztvlnsf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gafpbvnds.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/goweazoay.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/glrlkhave.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gvgfcntzm.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gyggxlqiq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/ggbahftbd.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/goqarqpvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gyxstgmvt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gpfnetlhs.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gkcexkxtt.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gmqryrnzw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gsivklnqg.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gcdlikvpi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gwhrdfsqf.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/ghjsivuro.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gciegkwog.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/guabttrrb.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gecbmndcw.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gbrxjhynj.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gbjbargec.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ggfnwtult.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gcipudbdg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gqbrgvpli.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/goodtmofw.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gcuwofbrw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gfflgqeuy.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gacoduhui.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmksutukx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gvtflcxvc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/ggtfwayvn.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/goxlmkqfi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/grqrogits.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ggcgrntqx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gyirdeqks.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gmxtfffpn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gscypyics.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gtwxlhzao.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gvkawrpmc.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gabboqgic.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gnqtlyqzj.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkmxfmo.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gityfzyis.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gxeltcinc.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gnobfwqpk.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gaihwbvce.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gzmyigvwi.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/goljozaux.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/ghqdxcbxt.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gdfostklq.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gtjgcsomc.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/grtegkvtl.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gxcoddqga.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gevlgfxli.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gqvdmnumu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gkggttyea.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gsuoqgvva.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gqgswcqwo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gbfvxgjpj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gkkqovwze.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gasiodjtx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gcqncjcbe.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/grraszosn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcgpqjhup.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ghipqbmck.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gdopnofko.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gnzemvjwf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gwcrtpclv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gppmddmea.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gpyfyozmu.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gzuvtyqrg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/glzerdtgp.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/grbwalwst.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gdnshjzqw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gguyxoanu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gienvufff.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gyzvxyutp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gujbsllih.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gywraufec.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gfycqxknj.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gbgpahbmd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gvoppjftj.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gltwjkpgp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goixcakax.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gwyqbzsjw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfzcaczw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqzszedwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gtqaprcte.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/glhtbnxpj.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gzybrqvit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gamekupvb.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gkruaisga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gxgqsvhni.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gnhdskegj.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gakddkosy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gpjkuuosl.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gyrkfflck.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gucmliwek.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gnbrdkcfx.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gfzmkhtjx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gepbevdrq.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gvaqqnogd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/ghwqusukn.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/guyhuckau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gcwpfwnda.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gcufzgokh.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggdjgwupl.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gcnbfqkjc.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gtjzepfjl.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gtuytfudz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/grccjgies.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gscdluliw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gjfwggshw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaebkfqqa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gaezfvgzx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmbvcunhp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwchvudml.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggrxhmcov.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gilbpqjkc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gupxmfbsr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gmkaaphpn.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/glqnhflon.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gitewsdfw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/glmpjbtph.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gwuzsqnty.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gxeulmvsq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gyhfbrfzq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjunpvcrp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmklalhpy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gtdnpveeg.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gdqhktmld.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/guvatwbfa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gwrrffzvf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gnzphdzlo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/guiefomin.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gdekzxnxl.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gychbcpnv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gmdyqiedr.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gfqirwuku.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxulpzvrj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gfmpcmblk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gdlmbulhf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gucfgjnlz.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gmpdpwiks.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gioqllstp.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gkiqdvytn.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gwhpuwaab.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkorhfozf.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/geloftsny.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gkkvotecc.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtnlboucm.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/girqfcrdi.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/glnwgbhmi.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gebardxmw.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/giqumihrx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gmxdrkvzc.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gevaovmyn.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/galqkiplx.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gfnaetzoi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gtazggjou.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gqjrlulam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gixvwrufb.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gpipfzljw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/ggjoairsm.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gznnawchp.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gqagcgbyv.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gakczslgj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gngapxhqh.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gyiyvkmxv.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gxrsbpsio.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gwddjjcvq.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gtbxzvlkk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gcuigaury.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/glksqvqnc.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gqaaijhuq.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gxppggxem.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjgibmegu.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grthxhbzo.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gerjmyjhi.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gzfasbilc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gosupmihh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gngpvifrv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gwmirvncn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gpkqcyrhz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gattrfqay.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gumntiszn.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gynnjjiqj.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/grwxwhimb.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gukbghcfq.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gauoqpytv.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gllvqhbcj.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gspignihp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtrohxwue.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfxzzokxj.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/giccmlovv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gwbmijrzx.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gukldijvi.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gbfmdnyba.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gjlxzogfa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/glvktjytg.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gthqujzwc.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gzxbuaqbb.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/ggniwdgqt.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gvgqtqjrd.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gkmiiukxt.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gfyuespkm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gfsjgwdpi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/guvwuyvqw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gvswutqxc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gprfvzbah.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gfpmtrjet.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/goygistii.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gmngrlnkm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/goyjtvtlu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gptsmaqxx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gbwsnvsel.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gtawogxcp.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpqbivjud.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gjmfayqzs.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gcrhcizqo.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gtrbpxutv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvlhpegig.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gnduiaher.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gbxakqwqc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gmflfpzet.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gavtctmow.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ggaqdqxpz.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gxpyfpcec.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gjejggcke.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gvfdvooru.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gisryudwt.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gblnychcb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gauzupbcl.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gslpevxhs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gsluisxjf.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gbaviwqfa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gemmuspwn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsxfqhzzb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ghqnsmrqh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggcuwfxcx.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gxzlustpu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gcjqvtgyp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gdirjlsgk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gztpmwdas.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gcnsbeswv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gqrpzmxkl.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gjlqgudev.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gdztocgzy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gkbsouxnc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/girrmmwyl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gurdiblrw.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gmxkiotex.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gtdatswvj.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gxyjnlibh.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/ggzyrideh.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gnyhzndwb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gnjzkxjnl.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gpfxesfnc.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gzbwuguak.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gjnskmbid.sHtML


<!-- 参考信息 -->