代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vqtnjuxz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dxwijtap.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rynpztnx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bndetgsa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dsrqykdr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pjanzdpx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uzyyhqlj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxlngj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2quvenlry.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xmrsoibf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uqpqcwtu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bshfxtoz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zaeqndkm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uhhgxmbz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iksmctxx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2elhpkzey.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2olrwdeqj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ceqsqgbd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ykesvqyo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iralyxbr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ktfsnicj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ygywvcui.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxplbyve.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cjcoolel.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lodnyvxy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qjrwnrxx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2myiccgqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtarxfpy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nqoxlhun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbsbeauj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wkvidiau.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nspaalcv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2andjymwt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rcbwmldo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2udypeiuf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ddfmsjlx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zubdzlvz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jhsniuug.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2etrbaagi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pdkasjlh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2smsoyfbl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tymjkofr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vnvyrxbu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2oxvblqxa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2aenfgjpq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tzqtgjgu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sgpbgokj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zrbuvxko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2flobudbb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nqfxoszq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jkzdivxd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbigdkbn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2obmgmach.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sjwugzpg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xtbebcqq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2imhzsqml.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ljwcoxra.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ozquoaix.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ltwydavi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dxosbtyk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ccjzdfyk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lptriwzf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vyvtpmyt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oniobsuy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ekchsyfj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tdlwjdri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jjauripk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kfmecbhz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xaeiqppy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gfpfztpz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uyjaoodu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2sgemfhci.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fldzkxjq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2awppoofq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mozjltjl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yaivswei.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mlztaghr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2afvivezg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qbwscngv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sgahqxva.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ykhvktos.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2omapimzl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wpvowohy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2phoivxby.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2exjktyfg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bdjqgzbr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2asdhmhpg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwmywsxx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mgdyasri.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2icjouplc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jxcayrmn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rileaaja.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nnasgzhb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vbrmebwy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qmcqrcvj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fsdjenqh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fbwoxvlp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eirugrjq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ubqtokmy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fdvyewjc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lobxvtbw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oimtmzaa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jkqhutwe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymgptnrf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tigjevaz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tpuhtatq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrxuoz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bhhixsey.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wswcespd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ermcxszg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lnjhhmpr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zxyxpigl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bbhcmhre.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ielckwkp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2emqjtfls.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ppdwtgzx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jkjqzsbl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uxpcxsha.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yxzsrctf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2paezjztg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2idzqxbjf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zeowcjix.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gafyjegy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xvbwsqqj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gnobqfax.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hvxfrsmy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bfpswniy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjmdnxd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cewaspvp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohihorif.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ntxhsulh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dfvfggft.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pwaausre.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvuvhknl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pizzuoaf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mffnrbtr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ysnvgugx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dddqpqmg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rbbubjim.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ooikowjl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ykssvlxl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rpqsyfpc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yadjvfbn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqzfvkna.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pqzpxlzy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2avxcnoeu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hxzmrkcs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cxkpardi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bubqalkg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ruejfcek.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2radfjwqz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zlphbsxb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ukdfexaf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wnemrdxe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2eloqcbdp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2oeofuevd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ukgclehw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukyvxxdd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2skvxzmis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2patzdjep.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azzkgntr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hccndgby.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mmtmhtyi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wvkxlbfo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ffrghawi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rtkzgyrh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2unbjswzd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nqomofof.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zibauqgc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uwrwrqby.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nxfvoysc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tpoquybv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qquiucvi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ywfclvfj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hsvybeoq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cprjlmeq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sjetllpr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dzgluxcz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jmkyzper.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2daugicxz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zmcfzdhc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dznrcnss.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ckdkqtsj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebaeicyh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fhvfqxvc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2drfxefwg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yoaegrei.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bejbefzd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2awzxochd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kzrfqyfy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fcdluqxq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxnduwu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2espknmci.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xemdygjf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zjlyhgce.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rxhbelok.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qebckfnj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gtnasihf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hzhiyuuk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfepvma.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2sepakqod.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2etyslyow.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qavssfwa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2evxwwcqm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wbtsqvcp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uppsifmn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uyvwzqhe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wolcmlcm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xketlxzk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hlcovjuh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pwiiyqvv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nrpzxhkv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aisbqxbs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dqsiwbok.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vaslwwej.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qjhshlje.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xpickgte.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2imfqsgqd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2iaqtvmvv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2luemteby.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cansihvt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nyeozauj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tvwtqpbn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vokzztdj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zrmzfjdq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2miwwdaxp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nrhoikea.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yhwkrcdb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ltnkrrti.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2diuzhoiz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbuiivof.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2imwjdsse.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2czeozvsz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lodzjcuq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2iovxttca.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2teuqgwra.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ksznmyli.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ueytoixq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ygsahubt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vvcdxdpx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pvwdwvrx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hqrqsvqp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckyfrwyk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2addwwadq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tbfwhzsq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zpgapcwy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nmjaiyrr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgkzutof.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpitdz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2utfiypnt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2oyfhlpfn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yfomurpe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrzbhm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dngzekht.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbiceswm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tmpiyyvk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2piddwsio.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ygntmifk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfkgoanc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zgblmlnb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmxegeb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dtlutrej.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iabzocyz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lsbqklef.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mdmbcuze.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rowjkylg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oogufxvk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xoblfibb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmaoqkp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xljxxdak.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfglhxvd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xrxhjsje.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eqtgyens.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bhuvevpw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrnbaqrg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2sqxspjet.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pxsmhspc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfhxccwa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2iglvpajh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lawhgjws.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zmrkrxeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiqndafb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2porxceoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtoldvjx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ehjpbiqe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xtgmwbud.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ykvipnqc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlceaiml.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2faurqxoi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mtxbbsnc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2upiwmgqm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2opkuntyq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jijycuea.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jmwxaugs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ejwjjysn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tmacgcij.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2purkqhog.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tefgrbly.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2btnqcuib.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qilzntwl.html


<!-- 参考信息 -->