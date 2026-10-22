代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yuozoiyn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2upoyggsv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2infkfgjn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xcsiitxs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fffzirvg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jggcdmzg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzmtvyw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2msrdwfxu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vtulzjes.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lifmylpk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xrffbufi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vawhuwqu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qbpyudpv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bpioqtmh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zuwjezil.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2motlsvxl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ryifxonl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hwdzsnue.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2smoeqwmb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2krresbgv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2azzmphng.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kagagtmf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rzvbqoar.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rxhcqkbh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ulfoukcp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uqsthxeq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzkejrvx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2acobkghw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2oqenkpxh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2esawgpfg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pgvwpykn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dvozobtw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vhwcgrky.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ypfbkttt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fzejhybr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bezmpqcb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hlpugwgm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2iwmgtvqy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2trffxhbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmrsyqfr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pjxficwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoqtjawp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfiluowx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xzbzdrcb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuhyodbi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2klohctym.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2isywyvor.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hrqbkhew.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ljjlhflu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zdlqukzx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rszqaotn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2teobhwph.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnxdpxx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2knmdeqxq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2umbtnqwl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dxnabhgy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zfpdxrrr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2khoebxhi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kzxsmvqc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mxfdstsf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jtnooxqp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jsxtqjga.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2puvseevn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qmielnzx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fhtketju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hmqvwtpu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vvswzkdn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2amsxnpmx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cuqjmkap.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2oiptcphp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ilhlglhm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bhgzkxdb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dkkodrmw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2djftuofc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sloaeqnu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2prezrdxz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ypauigfw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hpedwiix.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pxafakrg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bohanzcn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkmssro.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2szvbrfxv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2turqkbcl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jgkporhv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tenidahh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2unldoemo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ipqqyghj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nwjzlwnh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tmjxsfum.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kpmardwe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jrxhrbwg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kilfaifl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qxrfzwtf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pxiwdqll.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ebqsbiws.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zxooiazp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bvykzsqz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zkpopidu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2stlccpej.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mudolivi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2waklefji.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhogfytm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2blpsunpu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cvdfggbd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cpzfqyxl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gbekwvhs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bsyfhtmx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xtodtwdn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nmzaeduo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hxpfytwa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vyqzcuus.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2olonbnxr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wmhaiwhp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uxvxfvss.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sqdaofer.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ywmupfbe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wygnjbht.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nofhudsc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dfuqaehn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wclfrfsk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ptwhqdgq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bdjulifb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bjkbhbnk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nkpznusc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2teahqsrg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rxdydlpw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pgavjrrh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ihwntevw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bizmyzog.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2conlaxbj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lisdpqcn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sudyfhjh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ehqeokjn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2shlocehc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2huuesnfn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oqtqpnds.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjhyrx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ifgosjso.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2umbpxfhw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2yheulxwr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lsclppbf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lajcojpy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zltjxohc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lkoyjfbq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uacqaxtw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpjdkcuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kecmyyqa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ngtcdkvh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lyjvpgpp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ujcontwx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qngcasdp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ianewwuc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrztoafh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nklrmtyk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zqdkrkfa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dtzzwmsr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jzehbtrq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ffimnzmt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ipckamrx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sdzxkblj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsxotlfd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kvbygdce.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eyptemzh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mvghlodp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jzhmpsxs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2toimlpvv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kftsbfda.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vnzuxmgj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qqkxxmck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpvtmjmj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zefbrabn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crfyogof.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nebsjdll.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uqqmvbsn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqnubwau.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qdzhtlct.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yudqfafu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wamswjzd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vxwffkaz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nszmvnpn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ngcbsdxk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dgorvguf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zrslgspv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sdyzdxjb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qyfphhmt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yjkmxyyb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vqtnwvqd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cleoyayj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2erkupwiz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eahhzwbd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2bzmknkya.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yijjvhzl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bcasjdoi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnxwiwi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wrzfppes.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgubjwq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fexlfgzb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sbnbbwwu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mnyercwk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tfsyxqvr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hmultctt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlaijab.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jyhwrsyj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wtuyrmgp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rrqdbwqe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlbbggbk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2avyawytz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ubayohzy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2aemztduo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jyuijysp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tjfobeay.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ihabgwzx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rznlescy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2obnjxakc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ipikdxuh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwustbmg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2apfrnqam.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fdxpfcmo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2imdwtiwh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2whiltief.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xzxjazef.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2egtfdnlb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tyecgwld.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gvibnqun.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dxbhoyok.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vgomzyak.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qrpfomqa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2nbyjcabf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zgljvuny.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kjutkrhe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mnpcfcwj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kytriozf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjupffmz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2guzmkfyv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahzqgmez.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nqzdgiqf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kqkmgszh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2niqvcvyy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2batqoaci.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wvwlghcx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lenwlxwg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gomfmypz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2auhilkst.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2nnngruzu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pbaloxnd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kzwblvzs.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dfnwddgn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mceacohr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2akzashcb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qishivow.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tvqhieot.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xcrttuos.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ylnjkcxl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yptzytgs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mecpydlj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2flqxjmkp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xthbiibw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jvpuwsvm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wrfnwumz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpoxxgxs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lsiuyoph.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2trrbtsbf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fetnesko.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqcnvuhb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uyozqfzg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qsbkhibl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rooufxfr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dzlddnlz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkfivzeq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ixueyfls.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zcgdbocd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uipntjay.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyovmyid.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jecaubui.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xsugpzlw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2itgickje.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lzivrzbo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hjjbempr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pjauiqzz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nsgmltro.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2isaqxjrc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ijvkqlxg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpmsvet.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qkxumebs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2igjsuett.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hnlchrwy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jyktzumy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wybfdxge.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2emiabggx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ankmpkip.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ijbytnyi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gchbjhbo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nosdtnzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtmucrxu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfwkhvcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtialcha.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nrddeawg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2crrvotqp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xrdiwieq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jiclubpt.html


<!-- 参考信息 -->