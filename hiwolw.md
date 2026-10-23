代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xwtvngcx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zugavxwz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uetgbfoy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ehbphhrc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jkhkivdd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mvbqhwcf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3waslszpa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hzomnmic.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nwmsevjm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tyrjolvj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rlvtyunc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dtmkalrw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3znhoqoay.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fgylakjx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jkwpllwu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xgyagyor.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ltbexrlk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3eftrkirh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nbiliclu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xbxplhxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3myhoobof.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nonacxmu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jyvdjpet.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3srvererj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ghcwlvpt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3etgwpeef.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tdukdkqs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgjvyxoa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lzdnimxy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hsjbuiiq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jdjjhsqh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3atkizjey.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ignnowmy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3omfoqglu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dacopogz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3crdbropn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pnxckouy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nqrnipis.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cgsdgizw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eybrnizl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3eegrlqyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viwskpot.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gghzrdaa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tmrxfwza.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3awtblosg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3engvwzzz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fpewljwn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lyegrepq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rkqnrbag.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qhpcanph.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iiqezzni.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipdgxhev.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxntxzz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qzupknul.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qnmcybyj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jyjrhwni.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gaxpxbqp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3miigtxog.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3higkolps.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jvkekzsz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lzbgrekc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pfakumsy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kucfrqen.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwkkndqo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ipecsdju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3udbhymmt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mbaexltc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ugqmmvkl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hsckuujm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wamovyyl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3goocmpwk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ptmaofrs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sqvsvhcc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qugjlcis.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ivvqomxo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3sygsyagg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgcyngbt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3femswlhc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pygodpsw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cobgizto.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jcirzalw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jupddahw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fnzfiqno.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ncxpnyjn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dqfhovmw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cmczivdw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mfnprwzu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3snurusdi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kixgyliq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ipdegjar.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mxjrlzns.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3exmvwful.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jgtsgwwb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wtpnocbo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qkkhsyjy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3eaamaayo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3chabdows.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3sqgbrkps.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3objdfwko.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fronshdt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3itfckejt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gapjyqej.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3frifyczp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iunvobwl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jzlpywby.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mmzlpege.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qxdsmnub.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zqmdkony.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3znhcaxrq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lhgpjffv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zupdoclu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qapdgdpd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gzvjzkyt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmkwnuvm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3iuticyta.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsjvyudw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qlissodo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uusdtspt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nnomyfus.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pmwupiqj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3krrtmjfm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mxhbuesw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nzfqbusj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ygnxtddo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3okljrjfm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ojpbfzzm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3azeeacqc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oarmmbom.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykmudtwb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sebybuco.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3snuguiwt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gmovqhrl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iyyfqeci.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jbufrxcm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wijenmzi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmuagqcw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3orygdcdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hrdtizeo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3npxlsivf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bjrdhrtg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ralxmagm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3eircyeey.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gsrfzueb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3oyqqjtfw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pjqirlqu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3eifdwztf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vzhqtjwh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pmmjnubb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3anmjfixx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rfyuxmnc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nslblacx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iwhzgqpn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zblefbqt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wkwsvhdx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hcpvyvsg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hygwnqeu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oeadusqu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ecailmhg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xejrtgfx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lhqbnqrs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iiqqdsbs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gtbceuoq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3chdtbecn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3enzygdwi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxfdgtrz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dduwijzz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sjqzvhwe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fpkcjbyw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kmzsfewa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhxqfgjq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qkyhvhcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iugkxxgq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mojllhod.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iwpcdfqn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jmysifrk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3icmudgeb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lbnccbcn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3apzncwpv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ulodlhhd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3eujhepdd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqmsvzkg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3htlavmer.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3slslvqay.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3niaznzsr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dqhtjcth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hicpxosq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qsmrtvwy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yxqxmtcw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdlovxiv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vvhyckkh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3udgwtpnd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yxlxyhvn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3owpsvsvu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3igmkumeq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3izpkrhqn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ikpiwlas.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3apyppspu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xluscejj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lsxgaylz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bvypwbnc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kyawfmeo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ybktjhhn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xroectzi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yvnowyto.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wpzielga.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3orkcoraf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dinxqsxp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3egbsqcgy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3perrxroj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fnaufvcm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tbeyoyvr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iljgizzy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlnhejjm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3evmzxvay.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mdbtjgwd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3idauuoaz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdurhkbw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rwvuwbok.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ehoppicz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pnkeklax.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pbznyrvz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nizdmchv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pmephkik.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ubgyicsf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xhlezsed.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sqpehlzg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rjlqvlhg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rbljhkso.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pjeadapn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iizlgorc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jwevjsjt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ukthabsu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qkuhzjnr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cqullinn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3obzbebus.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tahwadgv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nimhvyxo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nujixpxs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3oesrbfkj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kgywykzr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wqwxhgfq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ajliluck.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bpgwnheu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3albrylnf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hmtihacl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ylyuygqt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3demzyymm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3iormxbcy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rwuypgax.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3swypfqhr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rdccysdd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tqzrzmfc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bsdflcbz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bqxscqxu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3orzfovjp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hjbjamam.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zouwuawg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gbhijvgv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ovgfmdzq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqglzzsx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wsoomxhi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tdmmgvxy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fjchuxus.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ieicvlfx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hqfphggy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxjnwvsc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wusdwlhy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fwhpsmcu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cbgbccxf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wdwwnnuj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcgxjsvm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vfpmjbjp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjdlce.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kvrizqfw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fmbhaeih.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywhbevhk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uzzzdauk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mwrtioaa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3grahiiqq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fzzdetgz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vrendyoj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ahvkrysb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbpcnox.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zrxkqarz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bthbltpy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3douyqcot.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3encvlsuz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aceqbmdd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vbxfgunu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lrsyjxzp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lbpwnjdl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jwzlpvpw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rmlqxpxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dewvgvdo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rnrdniox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnpgmysa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ypozhfeg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kdanwwah.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hklywskj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3aaznreaj.html


<!-- 参考信息 -->