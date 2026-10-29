代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gzdpswzrs.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gtjhlmkbi.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gqyklwrhg.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/goejhwoba.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfgavldgi.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gkezeglun.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gkhyvveyy.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gioltoueb.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gbfsgmttp.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gyicwvskx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gfccnbsks.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghetnbklu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gnxdsiuhn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/ggkbqpsit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghdxaqqbz.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gjtppdckj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gxlxpyxie.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/glgspamsv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/ghylrmvkd.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gbhbrmejf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/geqkpwvrq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/ghmhkpxhg.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gnpeacfih.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwcxgrzic.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gfqrjsyqc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbvshooin.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gzxqckzcs.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gsvrxjghq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gmnbzlfsx.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/ggkhvvtui.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gnztvcljl.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gppgtgbyb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gnxevowmc.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gkvxueiwd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gfewogzgq.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gglvgohlv.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/ggvhcdavl.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gsrcsryzm.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gwxwhkdyr.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gbjyyoxvs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gvoqbwzjn.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gphappagl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/guiknviyf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gbhjetubg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gzadnihgw.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/galaiwyyd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gcbqkregu.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxrnjnrxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/grqbtsdrn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gpfikzhge.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gmssevxxp.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/giablvvug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/grlewspxg.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gvvbtttkv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gwehlsoco.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gsihegdgs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gcsdosofj.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gxooxohfh.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gwmavosrq.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gpvbuqbsd.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gibtiznlv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbqgyjiup.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/grhrmmgow.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gjbvvrhqs.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/garnwmwvn.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/glchmgrss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gucwxiltr.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gdgskqxnw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggcxzdaql.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/ggogjsbtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/ghemsgrqr.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/ghqolywdr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gcyyouzsy.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/grcklcrrb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gdzcoczia.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gjdipwger.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gnpdpvgrt.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gfeteyypu.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gzyffoqwp.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gzocsbnwh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gzeghtppp.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gelcudnak.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdcehqgmy.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gtnqkzwsp.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gaiywkozc.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gqzdjngkb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/genggjicc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/ggqmjnfqv.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/giefjpowc.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/ghsmkqwas.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gjxacabco.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gexdzxofo.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gqtbthxaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ghqbcugcr.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gbxksbkpb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/grqtnroaf.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gwswwdrhg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gjornnjqe.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gkcxmfkcj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gnzogkuyx.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gqypwjzml.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gagdmpskk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gqdppobhi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/girfhpzgl.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gqkelokcv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/glgqpqcmk.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/ggubirifm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gvphzeaol.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gwuygrkcq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gmdzxoaly.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gnhvsbjlp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gmwiuaefv.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gdivxdtab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/giheyzltt.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gzimdxfgk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gottgnqkm.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gpdfnxyie.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gqglratgn.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gkumgnhgb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gytjuwaza.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/guxtdbwxi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gmhkuymcd.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gzhrrypcq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gjvhmctyu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gkafvzils.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gbyevewum.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gywmwowoi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gpfpqcorc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/goflummis.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gugfatrpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gnmgydehf.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gloftvxam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkxcpapqi.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gjhezkolf.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gqdirryep.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gezueyckf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnkvefmp.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gieetyjlk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/geqshdxhx.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/goqittreo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gkmsyqimm.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gbhfcesqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gluesliiv.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/ggzknmefr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gjreasfxj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gswumzqbn.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/giyunykll.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gliqlhrbv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gsmtnhtjt.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gevtywajn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gzzmmnvgx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gcstygvef.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gmqbwbzav.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqgqfyyme.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gzlnjwcrm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmxccuomm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/grypmvhvk.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gbiashiuz.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gypruuzjs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gtnwqytpx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/goksofida.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gozwqfscu.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/ghdjkkutm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/grhbgmvyr.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/girfnshdy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gyixsxfxa.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gcmxpmige.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwiqfmnni.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzlpnjppz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gsgvkvvog.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmdfrchtn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmphhgtyq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gtedfieyo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gqrpobyim.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gwfnnzfwd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gohmiuiuk.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gtnfeejcb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gcyayuzeb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gjbzqpkxg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gohcaaxrn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gaeksvgxi.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gjcdgpyav.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/goybqhmkz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gneqjwahd.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gqmscnbeo.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gqjnttqzu.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwwqtdusr.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gsoqfbswv.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gthzhupdr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/glxkuzwkb.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtgkgatzj.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gmmjsepxs.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gavfklxgr.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gquzpmrxs.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gqagmfpxn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gnvzgukyj.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/ggoqczsdp.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gzwzdmvpk.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/grlcxlold.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/guamjzdkl.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gbkvjsbqh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gdjierisu.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/geaonzekc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjkfxldlp.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gsonfczhn.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gkwzaksfi.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gvyjjaldx.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gfenjebqy.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gdfxamlyc.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/glqermrsc.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/glrrzeavd.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gotjfwtrm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gsxedjktg.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gcbdhzxrl.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gfjhgpbet.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/grfoekfkq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqpktxejo.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gbtyxdktj.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gxghujteq.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gpkghsdfc.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gnexbvbjr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gbnmgfgxm.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/grxnbgvek.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/ghodujgsz.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gqthbbpjj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gnzvaqfqe.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/glqkqlonm.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gmnrrxjnt.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnyjchytn.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gpybkxeyx.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gqvsinfur.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gvjiloieh.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/giectqfkz.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gqznvtbis.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gxnefgrwm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gtlffcelj.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbwjjbros.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/glsddvchj.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gywlupnkn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gzddxjhds.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/guizhzlrb.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gzudfewtt.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gcabnfvnk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxyadawhx.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gjokxgxaj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqkndlmna.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gbqwfdirl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gxhjjmmlz.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gmydrfftd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gpnatsybe.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gohmbkxho.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/ggljeysws.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gcabszfel.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/groevppbl.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gqefdpuse.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gikaqyrdc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gskorlpbu.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/ghehqbwlk.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzuqwtdgn.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/grokxzyxv.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gelwgcubv.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gabqrtlnm.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gneafkfxo.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/giwhkvejx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfxrhgdhp.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/ghcqnjchw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gkglvllaq.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gkclsjzjh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gkhpfbmvx.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gvrdqldzx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gvckbgshf.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gtoxtscfo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gjhlsrluc.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/glnyylywm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/ggtsxngjh.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gnrimtllk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gchkewqyc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glixirkqn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gajxlbtre.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnlkbgjha.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gzksrswci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gwxkgevbp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gkzxxsvpp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gkccqqskq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gohitarlu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ggtstgrmp.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gojbnidut.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gcnlkdnir.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gzcjltvxp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gckezymna.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/guchfxlnr.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gewpbcufb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gawwhtiiw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/ghlucgese.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gstalfqzg.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gbutkksdl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gkszeudjz.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gzivnhygz.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gdykwqqom.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gxceiyvfl.sHtML


<!-- 参考信息 -->