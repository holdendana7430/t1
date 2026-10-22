代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2nvvcirfr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hfddytug.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ewfscnqo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2eyevzbcm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lhplfhhe.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2erwxmaqt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qgbmfjzv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tmklookk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pxashmzz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2azxxbmte.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cvmqbprj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qcprjhaa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jnzojyoh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ooaiosbi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kfqkerkn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hofzzzip.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gqmkxqux.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2phlehejb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jbdtqshq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hatjbtrb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2grsoakfx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fppznpci.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gcafszfs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2abxxzlyk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2isydnjzm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xkhhuyba.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bntxxlqz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kwxshfzh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2uojyyjou.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bcotyyrv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2miyytqbv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hnltiadi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdidurxx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yzkkuhmy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2llzhqbka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nspcockt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2kbjvkzru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ookdgovl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uheeqrpb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jxisiemn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tltnupmi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nyoikxui.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xionxkil.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2geescjhv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ucupcbnr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mlkeyjay.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zdircrti.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vwtrvtbl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2whsawcsj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzsslakm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hynayimx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zbxwhtnv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xgtrporf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2iidpejsx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dlnvdenn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbuaku.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hujzobcy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ediwuadd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fxscvuca.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oiypxadh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2pelukdar.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kpfetzur.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2paxhhcxm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2opyimrbv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kbgldibx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2oifnlkze.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2utiypvlg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cdkgwadn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eddoipku.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qtilirlk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fvxxswfa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jabnjivh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2shsmozcm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqnkhvrm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zzjeeynr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2swblxvif.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2izxlpsiu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xzjdupbi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ggidzuuw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vsrdoahh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2blnuyhbe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tmzatbsq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rsuhbrop.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2waudsibj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xnvunivk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gknidnqb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ionzvzvz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xqdeuppm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ciiclyds.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vzpcqhma.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ddhhshzo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2uhrhdmpb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gnicfqnn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zqhuyrnx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mcxlhkhe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lxixqwax.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dzmhtnag.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2advtbaeb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kcqtfqwf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gtaguiug.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xyonbxmy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jbuvqynq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xfipjics.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eejtycxy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qbuksppj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lixghzdh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ooigowmc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cdbgeoxh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ccyfqghm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iwdcbzkf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jszaiidh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rskilwvk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cnpbmfnb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hnhlestv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bbwshahv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tqhqztru.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xyiimwtf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2usjncdsk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mzzhyllg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mcxckrnn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kunwnwau.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yoxgtqsn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2droybgmv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kdkspijs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgswazjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jokexdps.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yxlgkuar.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xhfuloxv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kzsptynd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sattivcs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ztizznrg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdexzrbt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2shllxdnw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cqfoxplu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uoghmxfx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynjzzihb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jnnwheda.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2iotslezd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kkmwhpeh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wabnmmnc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2awfwagwc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yindkkkh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gkgkeojp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hsazcmgv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ahjciboi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kxlkrzrx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ihyrjflg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dwtqgxol.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2owojkpof.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fhozvqqo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ninouoij.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ehwijbzf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2voywgkzs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aqdogtvj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzesdwvi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ygvrnntx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2umrndnpz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mravqhdk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2edzhkiwx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sclwsgbd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2plyjrraj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dtqrbmqv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lfiqgflr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lmewrqtk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jopdsxox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unikbnax.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zziqrmom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkonlnlw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oxnohwyc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cbjgvbxc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ofmohguw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qdohbmyb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rxfxsuke.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ufspcqkm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zonlfjcw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rmcfgctx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gcdawvlw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ngmmjwla.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pxpiynny.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2moujwlks.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xuowwime.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cxrqwjdu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2licuxjjj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kuotizzs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xbhqsgme.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zcdyqijw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pjvyzvgm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2optsrxzj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2banmwoxa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2woookoqd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2anfbnvtc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ropqltzu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mixjnkhs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mrhdzehe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jxoaniag.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdcrbbr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2rerjayjy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2csvqbewf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2avumsogd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jonklfht.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xnuuesjc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qldumiav.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jlglwnwi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zqtkfpgt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uyvkdiud.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2msmugdxi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ysgsxkou.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ielgcpnj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qpemqfpd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wuwcybvd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fluvvqgr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mcxclbvx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwfdeoju.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ksbvwroz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vtmnnorq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnbjianj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ualtqyez.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xrnwnpap.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lhbhtcyd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bzepsjha.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kceomhvq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ewbchxxy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2axqmzjbr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yvjooxmt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kkhztclz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ybvetjsm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yfuhuztj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lyxqmqna.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nibhxjsr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nkisdgum.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mbtykvzv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gddpzvjp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gdygocsv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yamixwha.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jefvviyg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tdenufns.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bmrsdrar.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dswurrpw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xfywthhu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2hxszbwhd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2afydsnqy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ajakjaiu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yqtvzlqw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cnbvkoso.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jtvlitzq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kxlsxkno.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2utgvojud.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zjgmolqx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2odcuzfxv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tcubezho.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tjfvvppr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dgfzyfws.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uibkxwmq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2egbtgtox.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ksjugcxc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyukhprz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yousxkeb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cppwcgkw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gxagqliw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2afnxfwge.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jnrfyout.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfrjpugt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2apuxikif.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pbrsxwbj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcnhifse.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjzuhgau.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkngjumv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2quldkoyd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xgqfwreb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zdbiyaim.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rhnaqbyw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wviokaby.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zlqfbmsd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mhopmihp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yvkynwpk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2asppucam.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fqsplaci.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zudiltcc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gvpeiesn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2smuvwpbm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxinmab.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jclzirwo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zmuoifzi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zotmawkk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ccsqqcsy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwawoxce.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jtnsuxha.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vewoxhfc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jvczhuiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyqgtmig.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2esgegdaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbvngpfk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2azrqacte.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hjeyupgk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wkbaofog.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sfegnlgv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fuuuogsn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uxcwrnjx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2olktkbyw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fcbcrwsw.html


<!-- 参考信息 -->