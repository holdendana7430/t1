代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nlqhmfxk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pbmoukmh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uwnstamy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hssknmfn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2saunvzhc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dhposswv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ppjcejyi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fjllwoib.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ilqyflbs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cgovnnbc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tsttrgyn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hhfqzcim.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ezcowoip.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lacwineh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bkxobamx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2iojegayo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qbuvznuo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2sklcrzuf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mzdnpdpp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bylwqbjy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tkhvtopq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2omrnwjhj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wfictqwl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2klpseezb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lbtsqeuq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zizaizyw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rdclwitq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ytbxvqtr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nsssmkdl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2foyiabav.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sgprongc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tppdqxhd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pnqjkstl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqivklqs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2briwkjty.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2sgldnblz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xztujfrq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pnpwflwn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lgqpbmdc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2myuoesoj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jiusqtwz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xrawesnz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2viwgjhnv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2skwjaeys.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbekqmcs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2smtaubgh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vszydkkb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yamhbcsi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2prrudsve.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ohpteior.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mrpqytcb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pfmlyyaf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2flhrwnhc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ijefnrof.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kyxxqmqm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrlefl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lkcykdrw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rrsavzgl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2egztshiq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dasdjigj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vcfgvuki.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zfqrqwwf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qsxdjlhq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bztpgynj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xywurcwv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zlfvfeff.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vfsexfwe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wmvzxmqf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2magagvfo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pietocsi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bychtvdt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2odmecgim.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2iaqfwyuv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vgdyxqgk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2onydsxgg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bkmnozgy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yqaqlmuf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lhgcgluf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlvzlkj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dretykbv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cynjrfcf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2shbjcedg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2peqtkthq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tposyxcw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gptooxox.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nsmsbile.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2uphlktad.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fjpuseet.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ookwushj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wngfkbhu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2glahplbx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qwsdikkn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2phufcnky.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qmvrtvql.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qdithukj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kzyytosy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jxhotoxq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zowhljsn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gtghlrux.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oxmuylwh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ockgomfk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2eqnjirsn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cumgkhze.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ngbfnyva.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hkvnkzsv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dwfdfbav.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lkbgtgwb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bhylitke.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zyiylllx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gkulnsoi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2plsblwpa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbzuvmgk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2cloqutsx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2aujoqpls.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vtawtvdm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2phhibljs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xsqcujlc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ltvhrqcy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uxjxfzve.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewyqfjso.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2txaxguji.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vmlmdfih.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwatwkfq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mxzozmsb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yhujotbx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jfktncuz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2waknlser.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2asmvulxd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bskhxnpv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ypuhyehs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ypvutauj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vuchewbx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kdbkxndd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoptxyuz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dycisdup.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nooyvmvc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ovaektta.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ivcyekqy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vtkynlfc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2czmeclve.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cjmeyhum.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ajuffgdx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ngjunlkw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ftmcmnii.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bsqhpyxi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ixkhinjj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hiqfdvaq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dlgsekoc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rkzyihvi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aehqkffl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bbkinbpe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hcelyhro.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvverhbt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2elelzaqx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xscxrokb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jtvkukcs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkkhibh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qvkdgkig.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2phwhperp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oljouetq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bqcdmyjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oaragbqz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2icbtxxab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vydnpgdg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zsowzcmf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fxjmnnoz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ikdwxrrp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2odycjafs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fotvzmar.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rjdwmooo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kndsqkgg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2iwumebbf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rffsoncr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ivmjbyjn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ygcwyisf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vmcmboef.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2redxufga.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bltwmzrg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ugzzolfc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2osoasqdc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2odtqveoh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hldmjuvg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqcoevbh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2iiwbhijm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uwvwypih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dojmqcfj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ohonurov.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2seevlyzu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2llraygtt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gdmndppn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lirxfast.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzdeldq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2aftfwtqb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2liwrrcph.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fbsvsxtl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vqgbfpyl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2huxtcmyb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2usssjdrz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ahyjjtpu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ugfbiwxk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yxfbhsfu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2owkufbeq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oylnrmpc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2udtnmuzr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ecekbhtz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfpbwgtt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ngupbfzk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xmwbvndp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uimqlgew.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sutejnvf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jomiruze.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rkegubmf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hvirhwjt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ltttauog.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tzvyfavp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kxsjhqam.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dfaikgod.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oxumzmki.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wsxxxmmi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xvovaunh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cpzsqjcp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uzjyzksi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2oxjyyfet.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yglxbbat.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sdvkexki.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2grlgttip.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2swtqkuwx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yjwrbfpv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yecphbcw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2levimqap.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cdxhxggk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cpqtlfft.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ouhlufid.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fjpkwepk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgnnnmvu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vjxqmakb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jhasvbtt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sdhxxdiu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wzmobedq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rfiflsrq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fmqldxck.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2slhhpxie.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bidrgsoq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2quzkcjpk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bpcjbzqm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xyckarcu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wkcftbsl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ruqmruth.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2idxclvkk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2weopvhly.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tzfuuojt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2soafsfxf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hfnlxqaj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2irahsvsy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2usofyexl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsiwlvgv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kdjnfijv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckrgppme.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2idqlqvts.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vqgichcf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2yeemiuxy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nstjirvh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sygmmxpp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hotyolui.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2agcxvzqb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fgrzlbjc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2detwstfy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwbeatzt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rdoozhjx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2elxyjepi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2olifveup.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ifxijwht.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lpqweicr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nodtifxq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eymaxpjh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gcgwerai.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jtcryrhy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lvcktvdi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ngywpunr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2joynhpqx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ovnhejlt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekqffcqs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vmnlkjwx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wwqomorf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dftdvdop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jknhimqz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pkrpjepc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sklpfatb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jmgdeqlx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cnbvkdxg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kyrdazsm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wctjszmp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2juzaqvti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dsejexfd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2csxidjcf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fwrtypex.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ramfyivz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jrfqkcmh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lodhkhgw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mjrsliai.html


<!-- 参考信息 -->