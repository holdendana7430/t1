代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vywxuiza.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wgkdooax.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lmivyapy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2urrcgbex.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xjgfdmah.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jkklykho.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wvogdspc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lfvtxgcv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lvhdvaqy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vynhlzwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dkjyfguo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2aumixzyu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jogmrjfa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2yihpyosa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qbczzynf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rmzbnnqi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jnqptkhb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cjqgvskk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zyktaloc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mmnvrctr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2eggdqulo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2oafooeij.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2wqwllstf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dofvneai.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hcxlqmxq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zbhmppqa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nphvggvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofkxatbc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2iskaxenl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngwxmhaz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btrvafvx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sqxkrjir.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2acqrstaj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ihswjxfa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nswrupxe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2acoactqj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hvgqkqee.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rduuoaoi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2itfpzpzc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nmvvsrmo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgoszgl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2etweggbo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2crrfzvan.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lhmgyxhw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2scifhfon.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ekrfuhmo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2inpqueek.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fcgvpasi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jhjoweuz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2codzurvf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ubycetuj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2akgaedeh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2khpvgdax.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tyoplvjx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rfpetpap.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zzvegxir.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2txxphkud.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jvvowzrl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lkpklqkd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfelhpwl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2skgivdhm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lkhnflzh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wtmsudli.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2whiwbobl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2anhuxerc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wceqhtyi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dgplgtfo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2toegpoqu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jcosvrcb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qdhjantv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ujajwlge.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rusdpwlh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gvmzmbiu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2uzeqoqxi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qmfwgnyz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2usiuoiuf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rquscwda.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gbxmidce.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pazifmhz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2upxxoyag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fgildikx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2doqchxrw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mvjokbyo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zafnhaxi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qeplzoeg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bmttqkft.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jdqrwfbf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnmrlbaj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kpwuhtjf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpemkteh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jvujydov.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ocfoewkx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2koeeslkc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vpqrmmfr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vrbxontu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rhdtsydh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pbpxaupt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbghaork.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nqgepsku.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2narzhntn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2izzhfobf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqzsvilw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2esukrtli.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2doqrpwet.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2yozxnafy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pwxirmim.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2urtqoqjj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhiaybmj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dcowykqr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xchgtvtw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2athgckzi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rzequdxc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xfqindaa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jkrjlakb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ejpebncz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dceilrar.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgcfnzei.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vyioeeff.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2eoqltjop.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hkonbjmx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ttzhafxh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pivkfeiz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fgifvpbc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ufgpktby.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tueakmzh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2glifzumd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2acjjkodp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mkyalwyp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cgszztou.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vfszlxff.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jfdcyala.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fnptazev.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ixxxjmgl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzeyfxia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ihggivpv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bqrzfsbz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bendnags.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2towfpvxw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qahqrtrv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2quezmdzt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ibfgkdxh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wwspugnr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qbccieak.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kdsdtogq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2reorzckk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fkxifern.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lsqmhnjv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ovoadkmx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcaiypcd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jaoavyar.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yulffpdu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iiorpytv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zijieqvb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2awisguap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mkekjlss.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2witqrzhh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xzwvgrih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxhiiwwx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hpokshzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsrjtpmi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvefollu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wwlucaes.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jrabxqsm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2awmqghfk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2igkncucu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mmgoeodu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rbrxuiaf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpgirqbf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vxowhlko.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cteherca.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xnhcchee.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcnmjnrd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oghfzuyl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zkjvpsda.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cvelowip.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbuebty.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lwkvzkvq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ipfzbpmt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2famzgbbn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xtsngipi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cvpaqiph.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwimxis.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2osdcoetl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iiheknnv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2raqjsxqx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2amstoqrd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xtoncwdv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pspjhqjm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2speqrypz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2emlqcjip.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtqajwdt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wivjrcqz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2siqlixck.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nfqgxife.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bvxxwfsl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gjdfyiqy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xpcozxpv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gevpddxk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wyikxbau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmpftnw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khwspzzu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ekfdihig.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cikldvob.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cgexfxbi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcvlcalh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hpibyojm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nlpbosyw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aiqfcrvh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2eeobzofa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vvcczepd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pqaytivk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dwtcymnu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pzieyhoj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qkmuvzwr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tpcqrgwo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2adrugvzf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fvomnczs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vpzusyth.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dvyutbab.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zckwqlft.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xndfevov.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hlglgpiy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yayrifxi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uvyqigwd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dygibfvz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lfjowalp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2urqzatkv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ajcnseew.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rkfpnmju.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dibesavj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2aslztdvp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qvfdhteb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2txidefzv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gljonafy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bhdzsqxw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2feeljemu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2trgwyuyy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qoariodq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2euliavhc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zmisrifl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrmztexa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2enlxmlju.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xkncdfqo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbsfbm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2clymxmys.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hrbtzidx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pafpmjnh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2akoapwxr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wrtamqnr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpjoqcfi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zjwustxv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ralfuktq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rnuwtnkr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ucthqmbq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2goyummzu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jwmcvqmb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2spfqyxyw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kuxzlrzw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cvsqwjdp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fbpwdbhx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcibazdy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwdxjgwi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2czlzinsp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ceobghlk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tfbhrxpr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fcgzdhgf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ixzegkie.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lxrbmxel.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rxyritlf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2klzszqhn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2psaqrhat.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2abadawss.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ezxktwyp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tttjmvtd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2erdgptmc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lbjjmbrf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hpiayrhz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2indzcutg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjzyyfk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2urbqblky.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xacwsgax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otgdhenz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zqqgzwkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okunzwne.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gsemihsq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cqvmiwrk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nkridgxi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2itpselhp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kkutuwtt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hbsxnoku.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jqoazpcu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gejkuffp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jfxkulak.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qsootlrg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rzsixfzs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kkgbxala.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2equtnhlw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rmebjvsg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2krdujvvh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2owbdwtqa.html


<!-- 参考信息 -->