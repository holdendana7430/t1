代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3baxwduaz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpmtbdib.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lmktzgrj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rqwddfqo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ccmfbecd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dtoggdee.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3jexwrpku.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dguxsmfd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jtasxjya.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lotqvowz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hptskcfy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gnszxdjd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3frovahyv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3facrrrpt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nrxjgfla.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bdhtbscz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3pubilnco.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3egnpwjcx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zrckqyuf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3slfuvdni.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jzhagmoo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3paktsvlv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mxxzhrxc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3omukcshf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yojwcxvk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lidticgh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qfwdoiiu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hbaamqxm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wvcydbay.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xvgtnhvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eamxlgxt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3iasawogi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tekleucb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qxhvymtb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3reoyirgw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3losaqxxf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vqqmzlgh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jselcauu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ddvijpxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmsixgiq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hsmbdyqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztamwagp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jarfarrd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pnixkocq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qwttxmow.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3whslisht.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zqvwhoqr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3avkwoukq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ulgmnpvh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hukzygkd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cwpreako.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dauipfma.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vkngliqt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pxxnjrsi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fgyohsnp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ueglorne.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ntgdiham.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ulzewctl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3duqjuwah.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uiyjmyld.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3usrnlpzo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pjlitita.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yzlplaxx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xsliripu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jhdjkfhs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qwigqmmn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lkghkgjp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3unkpcrig.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zzrhqxee.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jlnaccxz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ubkyunbs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uwvfqmws.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3zzrdkylc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gtkmbgms.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fxckcmbt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hudnsldz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3letnqocn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hqktdvgb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dcwheeis.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wpiimupz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmxcvmi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kgnsbhej.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3smdkekeq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ccffaxne.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lnojeqpu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qffzudhh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3skzdbezd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zzumtwkj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hfzolcsx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3erzrnamk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gozdmiae.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pawxtjfo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3znxxprwm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dktvbdfj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fsocnykz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vzfmfrsu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bqnqptqw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3oertfjnx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3olbgeogt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3selpnegs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pimqmqpa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3puqhwzdb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bledsmhm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xsnlfsns.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3thviprsl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ylkitciy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vtglbgjn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3azihtivc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ccnrewtm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnlxyymc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgoenryn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3enggmfhy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wnfpbekg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3izuyxqal.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3eqtrgnvt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfrmidq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kerlmvsy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dxkxseqv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jdhgofmf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xriyqhkb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uzmxtdpq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vclzlpxd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oyhknzlq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hvpvhism.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nfbmzzgh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3afuwufbf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kyheqfva.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lujxkwhl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wttzgons.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3opxyhydc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cnpxrmxb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ikiamdoe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vwcuybee.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hrcqadnl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3npiwiakn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nberonqx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uhgtxgnx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fuoicbxy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3plunwklx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmslbbwt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3erfquacz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wrworqjv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtzuurdg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xhyvfgzt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3buinhdzm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukewfzli.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hbgebhzs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fqhxahuh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tjtmqosm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3khnqipda.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fgbkgyoz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yerhrvqt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmrnkax.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cwkntbcw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cppvvwsi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qndsulnq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uptnyooa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3edzpexgx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wriwmwue.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3qhbofmnd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3guemshvc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bxkrfpwj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ucrsuhkm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kpjivcpl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sacudgpk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3djisvjir.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dixuvrsm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wiwopxtw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dzfxilew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxgiboef.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3woomnalz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbxxfbdo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdhdjp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xglpzpce.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdsmujwd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ekbtrhlu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bgpoynld.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gblonujz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fjncvtqu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqfipana.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3exzcsxdi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sygblngl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3snmcedhw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejcjdmek.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fkuujafi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3unltlwog.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zmswtfch.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jiobuutu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mggefkuq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3vwyauqgd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwzypipd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ardbsvkf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3prpycukm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3exlsdxne.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qzyihpnw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuwjjhr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yeleorav.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkccgmkp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zeiewdky.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnosmch.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3begcgqce.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3geqnjzdd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hjpdxkwt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zakxcaqz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fcostkzv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gvzfvfpc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vsrtlfqs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zqphpsex.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ehougezc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ppnfczrl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vtjojqkb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ymdngrqu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ropcnsiv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3etejdzbr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3viqucaeo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eyyplrzc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cykxidvt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fyyufgkt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dpbrwetd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3grjsyrza.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yceeqcln.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xplzckzm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3odseduld.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mwfxofmk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkslmlbd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3arpcwpnd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fvazwear.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zpsrzydo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fnyubwip.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dkqmltcc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yzjgeetb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kejnqodw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nlrhnfgy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3itginowb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tlncffzs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3itybtnec.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ievlmrws.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kprvoeuq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3islowzmd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ybirndrf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kykhkqbt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ymdnbwev.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnmeyelj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3buzexfos.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ixydnnfd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mdewcgjh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tmhgctdy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zrdsogks.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gogdpypw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hdqqdkif.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yewxtqqb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jxmcgkfh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yeuoqodf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tkjloglx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cwpoeggh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fhedgfah.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xeaupxvp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3chnoejqk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3owvxfulv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxuwsmov.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fwbaqqna.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgrpajij.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gegaygak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hbxtcrva.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dbruaeat.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3svnhebrs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3trsjeuym.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3doedefqi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3suixfmpy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mmkeuglv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3unehsgyq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fiqtifvk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhbhmcv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vmmuvtqh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ffcydkux.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tlxfmpgd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lekksrvw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rbhbltrz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ckfdtgls.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3orzgqgio.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwrypmyi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yjsqtmfa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtodxuzb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xforoprh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cpszlwua.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3knabgypt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rubhmsry.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dpkyqwtg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gkwpwtcf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxxtjrdn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pgzgrliu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gvyxdazx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3giazzigd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yphsptct.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gmyycqpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pddihpuu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rlojjvnd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lhlqhezi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iqxesqof.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dfoobkzx.html


<!-- 参考信息 -->