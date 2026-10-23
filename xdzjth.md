代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ennhrqur.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uluuagux.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3innytisk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wruurcae.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jsanfexf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wzrypswh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyhwdrlc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fkqcgrws.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fueyhdep.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nbojktrj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jmmseouq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ecnlvofr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gibqrkvd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gbddmsum.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tswjfcfv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aetfqqrc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ciowgpgo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zxanahbu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xrslkzau.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3thudsgug.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3goratvcy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cxpkbofu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wjsprbuv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3plbjzsex.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qwenlgeg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tggwyzjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kyhldkth.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3umhvroja.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ujkvmqzk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dgvpypar.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3oluesgcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebblspbt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3woyuitnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnjgzivo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3selrhlyd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zherbglm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xjijazbj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ekiydgjw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3azhjeacv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fnwygfrf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3saobooty.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fypjqaxm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3dnydjaan.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rbkddfjf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uombbqxw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wfqvcwda.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3veuatgqn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xniccfbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bjxtjtaq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ilhhjcte.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3athkrhsq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kvseangx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3okiistuu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3btpmvawr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zavyvvyp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3edgwyihh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ehycmvpn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3saekhvgq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ogiqmhyy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydfiwisy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wtbvkhcl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3miqzlgos.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lvpouvoy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kxlvjadj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gfclmwky.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3svmmduye.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3diswilji.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3brjzgtcf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cudvxqhc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hvzknaxf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3takhmscd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3waoamqyk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvxfuyf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3slwmjjpb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rdjzxewq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3muuelmel.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ckmxujsx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qlvyauhx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wnsdfhzo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uktsmlye.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ujswmnyf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3namleuwp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uqlpzlqy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sysxhizj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tffjxhry.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lnzrrsdu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dpvomndd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zquifjds.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hwztvkeg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vynvjdjs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cjzuijnt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwoteces.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zrgktztx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hxxyrjxw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nvmfvhtr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wyehomyn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lswgujqp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ylqacico.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dxcpzfvf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gphvbawt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lqoqlyqv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3eiaitjey.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ppfmawyv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kpgaadmi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fhtxbgbu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yyyiypsl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tatxbpdy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzlxhtma.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3chkztsxr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cslpkypx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uphxfsdm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgomolah.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rbgmtcmg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nshdcnpr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3czaoggii.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eiplkvsc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lkubcxth.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zijagquv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nxvfhkzp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxxgomda.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3djhccfbj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mlpzrvwn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqjnvupl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jdfqjknp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bcwdvkax.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mkarmbka.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ewozobkd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qczlmbbq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sehsorjy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3viotlfog.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3thfqqeeg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uuidkjwd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nejihlkr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfkbvnv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkmaktwu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3txvivdzh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jhbwoszf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qqhcbszf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nrosurvz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bihiwcnv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ettrxjfs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3diuoujqy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lkorvkxu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xicmtkwk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcugmpz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3visircvd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fynysacs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rioinmnk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vurknanl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nxaemerx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tjbyfesk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ttuznqfn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3putbpqub.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hrhcodbf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qatnwdjv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ccheckgx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hnyxlrxh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wgzydarx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rhydyudg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3llraimns.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ubxjtlsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilxfwmfs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3drugkoyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soaxzzyv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yqwirzdq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ecmdtxka.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhgzlpji.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uigjwevb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qxehtcez.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zrcymbup.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hjsanbtd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayychuzo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gjxcoosy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dikoyoui.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gaqumqpt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qnksgnke.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qduuward.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kasscwju.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hiodckpf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jowopgzo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gewtranw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gkwcnnus.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3sihlbfpg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bwdqvauy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bemghseb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3naqojeaw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nlabyjsf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llteuwld.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pvamwncu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hozqutyu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dddfeilo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xbommgwr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3cwwquwdw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sdnrpcgo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3blkxfqds.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sgpudfca.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3owbqowke.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uuquwatq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jswaosju.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tfesinns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fzduryrj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxylezyc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bjdsxwlr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fsluqofw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3leikttgr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3txcnvpza.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pytllcwg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gavdegxm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fyqchlqq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ulxlzoxk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cubijntv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3htuumpsz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3usniuzwq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wmmatkke.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dgvdudhj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wyjtjbth.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ahgiuwxk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lxueipip.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ytmcmdwu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iwqgepbr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qvnoxaxk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vemtftib.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jqxqhoal.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3givwzqjs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ziglrnam.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rrpnioxn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ilshvlnd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xyafriaw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3uowlcjpo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lalccmnt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gmwctelw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3oinmsodb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bjohdzxz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ijvmmixa.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3edojgngo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ldenjfzt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hbdutngo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3loajeksh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fxzxtdhl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dqngfdjf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qgeojrdw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oztkvdca.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jicuilbj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jdlxtbio.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ttnellrf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nnnxoulp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qbjwnkon.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ekgyxpta.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vprljjav.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fjcwsjpc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fnsybcgt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3htdsmkes.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kyzlugns.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fejxwkns.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3eznbqyul.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vmlsknbk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3eqhikwqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxfrtfyb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3omhmmsao.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xlgarpaa.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tiriglly.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eimqjlyz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cikdbsax.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3eesgfmnj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3evqcrurc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pvhcygjr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ttbpddwj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3muisxtmx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gmhqpita.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hrixrsau.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ixgvcyzi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dtwvpyvz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ibdfwzlm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ktbgszqm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mmgfsxjc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jlyqboyv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ekodlykx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mvltplfg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hocnsyvo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yxeivsvi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lplwmmlc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvhtoywa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bjoljbyr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pxddyfku.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aacwmjkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqyxfuer.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ttgwgzgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hurjlesz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qrqfrwto.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pdztmhxh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vlnmbesz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qzrdbeto.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wwytmsem.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nngmmfmz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tqabinnr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jjdwvzzp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ecqckmmx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tvushctq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fmnqjjaz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kgjxnwov.html


<!-- 参考信息 -->