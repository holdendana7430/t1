代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3utkatwdz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wxxdumbl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bdoydafc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ilayzlfj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3udfrmxjm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3irhgwyyb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tkxqfcyw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ytrnveiz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ezpazkkr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rljifdlf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3khtlhmuy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nsixrasz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bdnchpfl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fmfiweea.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nqbjfwzx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttujztkm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tdpnrbyr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3opregoyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3srcbducg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3akigajxg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pdacojpm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fuacebbe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ichgffjs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pxzuaazf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hscmybmw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3eknzbuns.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zveulxiw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nitlpfwd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bcmmjnid.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3alncalbu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3iimsenci.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vytfislg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlqycoqr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3aakphzjq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3httystlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jswsjqlb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fdakkwzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbntjcjk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fztlnxzq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rcbniufa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rwhzisau.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hpofgmqa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3saotfhqw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zfapqyzk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqorfe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rnpzurhy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3phlgocrq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tnjpcjgo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gxftzeqi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rhqjxwhp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rlcmthpw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dhqgoujw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ljohbkmr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3oloznxme.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rzxbrlxd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3podoqacs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hbobpjrg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zfnltqke.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3syvargaw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmvbvouo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xhjcfuxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dcegbvir.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3slqwibnf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xxjdqnuc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cpvpupmy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cwrvidpq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oxukakan.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vnwlxufu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ttzdmspl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jrbswimp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qymuzykm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qtrboxdg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ltldhefh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3byddcxnn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gztbqgno.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fjetfasq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ifsbjljs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cdpphcjt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3omwoxifj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yihzhkam.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3axvumxkm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cbtggwlc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nftgcuih.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3grlhdcle.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nllytygn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tdzmolqi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bmcfbqkx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3inhfudgx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hmyhsles.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vuuitblh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3eehntoaq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ihdmgydi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vgmblgue.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3avmpvehh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hkczfrpy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vjfjtxes.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3njhybaaa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcgoeaat.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oopmvujd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3goudxbwn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ajnqzrya.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ojewtsvo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vxjkmulp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kxwefloc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ojwspxov.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ugmckdew.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3blunquqn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ikaszxia.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xowwwwbw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jnddyicz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3litajncb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezvuutxc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3sdbxpcbk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bglzcjvl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lgdepkpv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oorrizov.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pxebxchm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kuuvfrwv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tzhsjuol.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eenbsnlt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3owoywvzw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ygexvlxk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hmlmgudt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wuogsocq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mdwjoryq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3onzcvvkw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fkoogaph.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vaepvtzm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ejqvleep.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ungkegqn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3npxpyryu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfatfzql.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lmtsmjia.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydvyumlc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qtrlkkka.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lowuvmip.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hzmflclh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gstiwlwn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqzspdvb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ltroyasd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ykshhvrc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ybxpkzim.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iecxxces.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3obhfqcws.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uiswokzb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtfdopio.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rwelktel.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jbqknlgd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mtjwqigd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3oqdopcgv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ukorxkcf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fcbxinzh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3elxoqxqj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bygsdsgz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wziaddcr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fcfusgie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbhdzuqj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3femynqfu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hhkaurfz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yldesyal.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dugrtalu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ptynuusb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dimdbyol.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hfvoloue.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ipienscd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvypjxsw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zaefvgke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfhtdrbe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vewxxpmx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bsdqprel.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yrjgtzmo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ulmkamcw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3oylvwmye.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jxzbtuwu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3caxubeel.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3imvtspra.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3oojaeovf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hlzihgdw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ldzgvnzv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3flzwxoxn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ezzrnsnb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3enmaxitw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3uzqypaow.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zifxdbzz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jqyhlmso.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cvefrgnu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zyqndeuc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wrvxdeqb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dgddtuyh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3miahugxq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3miectgcs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjedolxg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3sewrgokr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jlnsjbrh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iahrwwiw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lcygvmvc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hpxstxjr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3umnshnhk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ucjrqcqz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cqvnzrmd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xuvbskmz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vsxtckve.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hdcptabj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pazxzwsy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hmbafvjg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lhnopved.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hmflsuek.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ogixmpxa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3txjipvcc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrnixkh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gblbzito.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ewbukbwo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtpbpvbs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nggldcys.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kybsivsp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3infjrioc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3amzijlke.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3isfpdqfe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xklkvchb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ibnerkul.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fmprrzzs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3clvoigor.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3conrvaaw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pqvyudyr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vdnwfbjp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3caekcxgt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kiubftsd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qhwpcsvw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nrxeecyv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3akesjzyp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3orxdisxj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mvgfbdjw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mwnzqcpf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zywifvfp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fhniqrsp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3oauetrxw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yxyszmfu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3czgawnqm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ainjcahi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3syhlhgld.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hkvqhlog.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3phjraoqu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3maxpkvvi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hkrkmkbo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bxtukaqe.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3djobudgq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bkremfga.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zpfkrnta.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3grvenibj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vaatnfrl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3djhtdyqb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dctomqbj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xymlnoxs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3akomxsdm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eijdcevc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3omejqalm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rvyoiequ.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3peakufuz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3viiksgpe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wyqbtqis.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xsionfzb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dsylfjyq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mttlcrzu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3skujjpmf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwgvshwb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvnpejfp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qaezzufk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wvklldqh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cqpfzire.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ejcivkuq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3expldknz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nuuyhrbq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3indgzjec.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lezrqxec.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rapaycoa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gplmikff.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nheiisvy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tcsqwudw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxohcxm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nrevahqf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cknrgaog.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ztbzbrwq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixtgdbsw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zzihxtwz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vcftmwxq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qgrixeuy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3brdxmkrb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fwfvdxaw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbqxcta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwenycnk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wqfxabry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dawzufij.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rxecgqfm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xcbjywvw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3frfhxyxq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yknsheym.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ijabfwpf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3iyqabejn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3eysxaiwt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zcboptjp.html


<!-- 参考信息 -->