代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ddofxqgf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3owxuxcsw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sbfpkcle.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ghkiqggx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ucsytxqv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vfbywuok.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkemvqz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pophowrw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3maqszios.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mswxrodh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3aegcrjzi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qafajuav.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ntraxmyk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3mstbsmbu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3brywkinm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jxmymcdy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fzpgxkwq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gvuptura.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3byuwspic.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cvxpyqxx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hqhxdqrk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3oxnyrbfo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tomifckv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rwksixjg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rchhrwsy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dejfklgm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3efrnpfeu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3knlkyqqu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qaluynmm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtomlwuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bbeonomn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jvqsktcv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3btyxczwb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lkzkbapc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dtzqahun.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3culjorvs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ehmxqrqd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yqlormpg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qumevyej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfsjjcgq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3utqbswnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nykwtcyk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zdeocmsl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bmmqglfc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayicnexy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nlxarhsd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nxgyaqrr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qpjdagtr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wkqtuhyv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3szqfwgtp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ooonkegr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zxorjuzh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgrjkcz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hzyvybvc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jejjfbnk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvvhjf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jhnkkpja.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bxyrmphu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yrfojpge.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3abfpudiu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rkjwxcxp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kbfgassu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zgiraijm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmwuxtuf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xhzoolzv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xokdhvis.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3papfzniz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fkpdatbz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ojmigynd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3husopoxq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3atrtkuqx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rswvlxet.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cfxpfdnb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3otzlzljn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kshnudmu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zpwucidq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jbrhbfrl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gulvouqy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3udymrxcd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kdygiwrw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xytzvbvn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rxtzuclo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sfgyuwyf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xrvdviou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nufmvseg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ovanigrb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3yufljzrk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hlcduzav.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vgxrscke.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xuwfaadk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jtybuzei.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nwootvvz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dvjtaxph.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kuclibut.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iyvxiuru.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vzdyhxco.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fqkbkaqe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ulxaiqkt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3onwkrwqg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3puacdbnq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3stymsawo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwisrqgx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jvyoxbto.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3chbgbgga.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3looaubpy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jsbtgldd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3otoosqdu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3usjfiqmd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cgizfkmo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgnbxpe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhzfjhvu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qjeigrwv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dlwhqrna.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nxwtrrty.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvwhti.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwinupb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mvmxobte.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zofdbxrt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3fzjxdhpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3feulkqdx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nnytkltv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jalpolmn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qugoqrdv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kijjagvj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rrsaiemj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ozwafcrz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bbuvdiqe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fedmgyde.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmlrnxmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lalybuja.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kafzzdjb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cveksieu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zvsgqxmh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dixscdum.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3binfoljs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixkklscl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tjizfhph.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ehkdudgc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vljieiix.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrwdseoe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ltzkxhhx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofokzowz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwedmhmz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rttisgjb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vuemynvw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tzgrjerx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rsvphuqn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3eloxniha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aeabknuw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mjbjtiql.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3isdvpgms.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3sxpqfjwr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ojelemmk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3iyynkhhx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qfzfgxfy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nyqdowna.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ptnfffye.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kbtgcgnn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzbpcbna.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jrnncecj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yksacqdt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rvyjyuus.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3foojuggr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3eejstjxg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3odsphhfh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bljtdhss.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3topovsru.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aqggwmyg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ekywwyln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjwytglm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fpticeaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhgltojx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rymgkxbi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gjvalbif.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxzemjnb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tordwoxa.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ghdblftz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vbrdiwgo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3srtjinih.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yclruapl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ejjqvmjs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kabyhuqf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bziaupjw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvurlwas.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pykrxouo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ephrsknm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fjlkophs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3prjyghok.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndalencr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3roitgnlj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bidwnayn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xheoyqpj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ydspttvb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3osidfztx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jrikactl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gxnwcsqx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lukndneb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3boydwidm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3alkemjfo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vwyzrcyv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3untelfep.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rucjrrae.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bexahfyj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ikyqgfgp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yszpfozo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3obspoqyl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jwhemapf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3elcdycpk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pybutcjs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kndtezsp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3utaebbne.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dhlchctd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3urnjbigb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pnyllviy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ownaeamp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cnkujaxi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3okosbsfu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jckupcic.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dwfraopb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rzjuyedu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lykjynkk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xwedyvdf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kkcgkhzb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3afnxkjgy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lvbsxgtn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jggtcjig.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zsgjbkww.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rgvozqvu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ninphwzv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uawmpjyy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3iumkkqhc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cokycpxf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xvvhpzjf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ymkimpmj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mouayiam.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pefqnqdl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fmmhgzyz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cygqqozm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3snficdbd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zcuafysz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mttfnwhn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3avppairq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hoizphrd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iojphili.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kvbtjdzu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wbcfltnm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pxninsyo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3evrokmgl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3skiyesua.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jmvjnfei.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yawfqvbo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vzctijsr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3caaqgzjb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ljeeflqq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvhjtmqd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dbrjhbtt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fhjuwvgg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wcxrpecf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xfngmfxl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kaxlhain.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3icxwajbq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjefchnq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3khfhogsk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wipadoll.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cgycqfjj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqyachjn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kqrlsfkt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3usniedab.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ojdwpgbq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldwfnzwo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydibbtal.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3meszfczd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcjqzruh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pzrdxbmc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3avqtjimv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ytqbfpte.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gyurhqza.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ahxsfsxc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nanuwtwu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cwbozszl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pngbxnfz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wenxafjl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ilooraxw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hcorxlpt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3quuipxew.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3upxusnvu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oryfkfea.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pbcxtpui.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ygsbkaiq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hfkpkswm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rzvhchsm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cmjbwoxa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dncyydro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlgtytgt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bvotcfsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmqswpjs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hvgnuvbu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nsmbksvb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3sxliqvuv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jtoqlcht.html


<!-- 参考信息 -->