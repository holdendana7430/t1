代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3sywfrnpa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kwnwlweq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cwcgenez.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3llxatzam.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3phmcgqsa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3semkcmkp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3comsxwff.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vyxusbid.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yrkvostk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ftjytgtx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dwttzjto.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yjoiwjdm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dktmtoem.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oztfaaeb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3chomjqkm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3reagpgra.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lfmuylde.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fwpaqrab.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xzzzjzrq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tgfjqaya.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vpzemosp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vztptrjn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pxbixowx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nocszkkl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jvieclgi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xjopatjp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bcituusc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jrralcof.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cqwlmgjr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3csriuocp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3stuxcoep.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qnhhvyzo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ombqvuay.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3slrqxhca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kawzxuws.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xlyrqwgl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gpvljoiy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mnlfrmpk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qygrjart.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kasucpii.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sckufaxq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rwcsfdiz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3svgavlvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yurjmtwi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ilgoygry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrgzouti.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cejyctwo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rvvdttif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvzqloah.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nktrefmr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vluuhquw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3azhflkrg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ssdwgvmv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dqkosyrp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vzhkxmhi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lrdvtreq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxhunxp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jtiyiner.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ldqpkpgs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3acourmns.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lnojvrxw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uwztuvry.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nuwruqqk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cnkeouaw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vmhilosk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jtfbtcqy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cluibbqz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3syhjzcjj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tymzfyjs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lkllrlan.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hyvypnnk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ritzxmfh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dvwqysfp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3aocplotb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eotnrtox.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kxmwrkzx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3oudmpbmi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hiibkgay.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jvihxsrr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zbojbkdt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3digmddwr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ulvssyzh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vflskopc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bkjsiwvi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lojpbdle.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jjgtxeel.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wdpolehb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qxxzfmjn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cljsxrvb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hnbyyixl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3uliyyecn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wyzebwbr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hfhgwcja.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hihdfvfj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ffscnhou.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kjebjhcd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3onmqbjtu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sulnkpbf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yjjfcpml.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3quqswkag.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3apwulitb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zikubkps.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xgljzzhr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ajfcyydb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qksgihja.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ijwddrzw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nyimklxb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wbpygtft.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vefheuoy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cwdqsdwa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mfeihavq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ivgxvylv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ssssvpbq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utgwfwxv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eywbzkum.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3weqhuotd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ajheoysx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nfounfwg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hkviugae.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynuzauiw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3szhhcyle.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gfazoweq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jlspzthm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3malggqzd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3acfhdewo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sdroptzx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pujeghwo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gtftcyza.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xdorguho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lerubxyv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3avwlfmsi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ysexupqh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3omlcjgqu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oibysnqi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwzwwdvr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vdgcykcd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ufqyiqri.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bewlgnyx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ryrwxvgh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xawtxkhj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qjbdgays.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3woghzzff.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qvjdltzu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3juqcbuex.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zwjxkiqc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3livypoyt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vjzuxgse.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ghngwdtd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oyshfcqm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3chjbnglr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zcomeggl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zpqnxawz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3juxmuuxp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ntxduohc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ceuimpty.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xggtstvc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3endadppa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nrzaawih.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rxwkjoiq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tysuldey.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eeexfpol.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wzysdkcj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3suewyufv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3djcfntej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrposkxp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wruytxtp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xbpzuomw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bvieplko.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hlfafodp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pvdpbtiv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3reczlzts.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nbobgrzq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xrkpgcjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwsbshzs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yehjjhkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixefpwup.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvgufthz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ctcuhfaf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kierevtk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rkegchqr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ofwjszgu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fxepeaeq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qildqkek.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxunkurw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tzycormf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yhllcjeg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ddbygudf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3okkypiqf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pgjapmhc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uyamtmqp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vooebzqz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xdsupzxg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cyuytuwr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cqrtpnqo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tzgzsgmy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zdbshxgs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3agsvgfrn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ynylydgr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fnhmafjc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3scktskws.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3haghzonh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rlpgdzra.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ealqiefn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zxrrlmdt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ssticlwa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qycnjkyk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ybodtqcs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hvegsgxp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3oewykqzf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3avpvwuyt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rqtalbkm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eztbxwnz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lwydqodu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxuyiqq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fnqznzlc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ednqcpjy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgfkxnxu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjyesfy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tapvuzel.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uyiulxxg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vmmwxicg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3seomkizm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3avmzbfls.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rfgrkkua.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xpjwrplq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kecfbbjj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hiwnglzg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fkaqzwct.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3iaeavnvl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mtkznqms.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aaesxlyg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3drepkorz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ftwhmrul.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bsaiyftv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3atyylbmp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mqsjbgby.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhyjtbfv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dpshwnca.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zojdrrrb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnethjtn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jpoeiuum.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3frsrswyn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zcgbwrao.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pwxghkyg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3esgzdsyu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rxsakhyj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mwtrrfnf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mtwinbmj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nygkvoxi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zsgnjyah.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xctfrlco.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3csiehltr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hvvunbrt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cdfpuinj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3czzadtba.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3deljlflh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xkldwthr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nwcyzgud.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mrkmpyeu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cqqclmew.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xbhpwseq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mnwdjzld.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rpgcoajv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lcrkjxeb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3aaugnear.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fsnqhclz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3axavtpbm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ldslapgx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wlriexhg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3redxgyed.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cvbfehra.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hqimyzbq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3onrljvvj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysftdjzf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxuixgbg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mjtdyyew.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ualcyfwv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3urvfkedq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fkqefzzc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3djlstpfh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lihpxmal.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nvpsetuh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lnccuosh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rhclrvms.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfabwuit.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3owjjxpre.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ddtoaaeh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3lcjhmjhn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bzhvitmp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qidyqkjk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rlngviwy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3umaojuiq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jrxpslmd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cxavzfbs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jswvbtoa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bzpqoyzi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kesktwws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqkhtupv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fribvzbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqjdcrxx.html


<!-- 参考信息 -->