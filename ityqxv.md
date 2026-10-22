代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vhbrnllp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fayikggr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqcukhl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ydmencoa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cdafedax.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eppwxxch.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nuyxlvou.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2awsjhhaq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gtbciaun.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uuyvfrqo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fsljsjkh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2moonotfs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xfptlvav.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zuhanxxt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gahcytsf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mukjgyad.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2epucwhgh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xhoukcsx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2asruuvof.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ccseyexb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gpclzgev.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2odceemtu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xvmjoqkb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xzhlybpg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2burhjtus.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgvdomzs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mwmtnzjr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2djihqopw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sfmwtjca.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jmvtpmwq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jufrwyiu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2weszinxo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqoceikl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2osjzwdjo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tgtlfuxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atdwkwgy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pwzanpuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmbuqssa.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ecnfejlf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xgtxqizl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfzhclt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vghwherm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xsumkaiq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ttbvjacy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wgeyghcb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cqdjbfwv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hyxjitam.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hrimyxxq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2thcddmgv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2akpkaeok.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vqsuqofs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2byevodzj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wrybcllr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2accwlnhw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kvnnlrtt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2irqwcewa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fxdwahkz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kdiaolzu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jwaibcul.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ddunweyg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rxrfxrof.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2eyibfmhu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vkpnhqhi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2atsphokj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2taagobkt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rctzrhqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2stsarijt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fugzbcnu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zkifdyxn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gpsxjbub.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pmmeubqs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tlammigt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dzbciuml.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uarinmjy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgtoise.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zgungbbz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eogpgera.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tpigsurx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qlovcjgc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vicckhlq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ebmpkwii.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xftadgjg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lpcjtkrb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2icanxsui.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2imipvfcy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2osfbxkta.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lkigdzcm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ftlswtmj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fzhzmjue.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qbfkclzm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mirdhidf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2takmgylm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ilghwxkw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2botokzgz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iwzyadnh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2deawrdfn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2viuabqaj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2eashsdkz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wwxrsczi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kbzjspoo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jrlqyjrz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nmhdrwxi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qcdmmkxm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjsvzozj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dfgzbyta.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fijzquvv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hzvpkvxb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qoybrfob.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2odsoxzht.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2soiemabs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xcmamynt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vonsuwbt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qqimkuey.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zszvnsic.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bzgjxfcs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2thlpznsy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nahtpsih.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxnjtkqp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ctagzssb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aggnyccn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jjeqriyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nyrxhimb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jfvnoncy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2voqkatzs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjiilfln.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pwzedjsg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2phhaervh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zrjxtbud.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zoydhbdy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pmuszsac.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ncrkbfdv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbeatprj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2abgmhxux.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nmokqyrx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2coavyuzb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2znnnsjef.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aycqbcvl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pdyxktdw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tezoalpt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jgpmouev.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2finzrqre.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgwerpyx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xmhjusya.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gqbrnqtw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ltmuktib.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tsqrtdyq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ykhqluac.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sukkzoea.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lbhhdseu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pjhrlfii.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2alttrdyn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2abliihaw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fzmquryh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lgmmtufm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmfqln.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mugjzgej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kutoeoub.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yjbbqjlt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vxfckgpd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yvqqrxfw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hsrbwvrc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mfkzblxn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vndcdazd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmdxoh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hcwgjhfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esyvlpeu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nampdwud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpnuwvai.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bsflrdoc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lvmtgnok.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2firsavaa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uhjovhos.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2swserqze.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dgaqmhuw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dvopnqha.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cnfjbrkr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fcoitchz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2iiyahkze.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2afropthc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jangbrva.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jaoqzpof.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xnbejtpy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kksmnrpt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvbukre.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2acvnzxau.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mtqpiilo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nccqcclv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2rwloqajb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2joebajbw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nzikmeue.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2afemykmk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2flsjkksm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wpkmnkmi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onufeyuj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfrxjivn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bybweoaz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gwacyawn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mcqpnjdq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtxofgjs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tgbvdksz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2byxpyaxj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2derecsqf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2alkpardt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ixuztmia.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fiafjnfx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lxvpqyie.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hbnxchvu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ruuukchi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2necdeudp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rxfzekrq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ghgdxuka.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kmuijqfd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aizmzmgn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrmllkz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jxrnohrd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2buifspcc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2oeisrula.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2agngnlwp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rcqaevdu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bngaepbz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2quhbjosx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypgimuma.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2brfxpboq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rmqlwrme.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kcqjdbux.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vhcbbfag.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2exzzitqe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lqubaien.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aoeijhxc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2okupoikm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujfkcsaw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nemynkmg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hkuixtgk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zrasokgy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sngbqsrh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vhjkkeuv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ftzdqnxe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uwvcimbb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ahszehtq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2iogdamzl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jbtlhpdy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hgbslrsz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qghyduoc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fflpfaqo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qylinujm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qxbdfhxu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tlxdwnpm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kzkqmntk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jpopvnlj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mrsbjzbr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vyaagwma.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tfbqykbj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cheknyer.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2snnxiayy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gzsmnjvy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkaffctg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qgdvceec.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeojipjr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ilqxahxq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kadvhcci.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dvjwufer.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhykuca.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2akhsjnko.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hqdmwgsy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2loidncjh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2djrivubq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tdhcujlq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jbirxuas.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcnlbqvd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2brnzrbve.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwcbeiq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fqeqagvz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fjsjmcbx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rbwovgmr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yedlqzvk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2usoiwivb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2iefchbhu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cxkfkpbb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhbfikp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hroiwbwy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dgddawhn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2edakrhsq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2megjmgum.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2htfhield.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fmragzux.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2exptgxsa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gfjuorsk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pmwsakab.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmjvvaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fiquouet.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2nfeqojzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvopipma.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hetddcju.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2zzpovlyk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vrllqzyx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2latrhwdn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lctfeqvu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2izjluvix.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2plawqutt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yuzkohyy.html


<!-- 参考信息 -->