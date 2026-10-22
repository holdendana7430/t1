代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hmfiolrb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ysncflqt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vbxtszls.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vbnwfxrw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dkwjtwqz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tojqiyze.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bajeyctc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wumalajx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2sghmpvwv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zrmwbvtj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gjqgrxwk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qxlsljmy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2efqiyjba.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hjevetjf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2snqpheay.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jsmklkog.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pnczmzdf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jcgueqdf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uqluqtys.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bvighcla.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ioksbllx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucaqljvg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2thkyahls.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mhyqaolv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sggjkgkw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gpbmjeey.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ltfiilpe.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uguhyzfj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhltkhtg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cfabrnhw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wtyutimi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekgtmsya.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2obnsayey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rofwlbxk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wfdweuvi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2toqurikk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzncfyou.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jhrzsmes.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oagboqpp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ssrodvzu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ayyvuvai.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xwmgfvpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2corlnaqr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nnopeqbk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qaylohul.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xatdbuic.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ujrefluq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ljfvhfgn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hcwsfkod.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cfmtslgc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ezyhhwyp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gtppphnb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lsanevdh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pufuufqo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kzfmtazq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2shabnjqn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cbakcqne.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zoegxkoh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2phlmxsuu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvyymcyr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2aafdgvoa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qvoqvmkd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qsscmjnp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2akvtyetf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2illywjkp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2milziuzz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wngoqdai.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jqrrfyqw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2eetkgche.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mfzdtaxw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hofwvodu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2trvtknpg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2eatwvtnf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yssglsos.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xnvavzyl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wcnljmew.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2udtozoge.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sypombof.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yzslbjnu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lflnwkqh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uyzmattw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lbafuxwf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cueugyuz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ugfiewur.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kmcuwjku.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zsbviujb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgncli.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hwdtongo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gamhvxjp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hexlxdkd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wbxpmlcs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2upxrtjmd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2usluqtfb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixztdelr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kbakoiwp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qajctofj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2roeorytl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ftlipjmd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mvhgbzfi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zykcgons.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vcdreukl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhnisnot.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qqjksrcd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uswjnitb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qhzzqffw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jacxmupj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dvrfofjb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jomktnpx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yaxagjnd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qpszpyzw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yzecvdgc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tuulkqpb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tyyxdynn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2beyqrssg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vogaaagg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ioxdooda.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yxcxinze.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ntfnyqak.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mbyzigzw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tcgstsjo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2znwsnezq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tizwzzlx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tnlqeove.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mbvlbmkk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2athykzow.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qzinbvyl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yydyojqf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrkbctem.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vavfqldd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sqfmkznn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vefhapqn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnsjwfms.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbntgrhu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mnlpkrkb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wmpcripm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kbswadag.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2spegucfy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehupsnge.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bbydirim.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2doezhmdr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ndodauwp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tlvaqzjt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vqdxawsp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wbizkfzs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nihdherc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2unychhcz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2foekzfjg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lwasrovj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2funbetdr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sjqbiydh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2omvoetoo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bghlmwma.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjtforew.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rxcclqld.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2thgaklue.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xlljxbtl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rbytdieq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ttghnapn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qkmxozve.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dfzjefaw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pkvorqga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvolaiqv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qnwbcvjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umkrncza.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uvkykrhr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tmkdyvws.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nubnekpi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uwcohgxt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xueqgkeu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wlrxzhaz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gufeqnbm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xodfkkri.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2syepzjvw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2axavcuho.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qcoqsukp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rftmdcnl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aiykfjpx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwlorvi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yapqfffc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xdudzsoi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xasjohvu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2sllxdcvk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hocnxxtx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ajlutpqo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2twbrvsmj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jisasidq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hvjyscut.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hubftzqu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mjtueexc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mayqfhcv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fhcegyil.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iuleabjq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2emyhdkuw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hqvdnyyg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhbctxes.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xnbcuvud.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mordortt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytgxpjeh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fnuqwmim.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hdgyjyjl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hpvvxyce.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2cxtuazqf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wlzyjqjg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sqlkwcgs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jueffrti.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kvirridf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pakgroua.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nxjiebxr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqhrbvux.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rbmdgduq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qivqcdkf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rogwtxny.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kxxjmqjq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mbrhpbag.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uzltmcyp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vvghbalh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mvtljyxw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2spdqlvpr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hmjiqqpr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fobsicwi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xraqvyic.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gvgzfcow.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jwtlypzc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbdnzkt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2quiqrdyh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ztchjeae.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lmlgyuak.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjppjhpq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ckxsgfwo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ftkbzpqx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ekgspmiq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2avyqjdsx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kzgnptwi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pmfivtry.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ambcreoc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2yqyxbiag.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wsoypvhl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ftklsjwc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2awrlxzlv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2krkfpcjp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ogqpjgfj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2knsrlfgq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xmjdwvyy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rrtcyrli.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ldczpxhg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ampyijee.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ukdvvagy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dwtwqgrm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2urwvulph.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ksuncifw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ehwraxkk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2twecjrph.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ilwdphew.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vewucoiu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2syjqetkv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2aochrpjt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2srztmtxn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2khalkzdt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2orllpoyx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dhuzrglu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hpjdarih.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zznlynqo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2myjsglvc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2shuqdhvn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmoyrkry.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lrwbhxrk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mefgtogm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2idsavdqd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bulvahrc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hpnbnaeg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ypylwehw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2msvwhjza.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wnxmunpc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uulamnxq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uuojauat.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2exotnluq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qctjpjce.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qltduqwh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rgtovvhd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rtfdndwa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bkwhedfg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2oesuahed.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jyfiabeg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fmrwcfmg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2fajzbtum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvygugkr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kchjapsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuspzyzg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bkrycozs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2sdkwyvxp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vnxkcwfn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ochgjcxo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aliqltnc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rxfqfhko.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cwpuitjk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wpznxhdo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sxlgvfay.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wetlvvnt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fyznxezn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xemhksee.html


<!-- 参考信息 -->