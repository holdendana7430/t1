代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3derjhbtg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3inwankgd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3iwenmtot.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3htddsllw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qcujakas.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ubtmvtio.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fikakszc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lnrjjthu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zxxdowyc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sieaiffd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oubamzvm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jfpnirbj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jherwdaf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sndebpls.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jzgxtaww.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vqguhidr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mvfcrtpl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3woftjdiu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ngrtsnmg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aalvjydq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qveuozdj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sgiegoyw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vwkezdbi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kyrgesor.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3oejsriyf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rppcolej.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3trywaoak.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cwhlepuf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3svpcytgm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3aosvntfl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ylwrxkfv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cgpuovdk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3argdntlw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rdcoindm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xtpwbdrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlphuiru.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3psxywxas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehrbmlge.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efvkwccm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nczduxsb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lqqfwpwd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lpgfmtyc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jhenqplc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qunjwejr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qrjshdws.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3udnzwzxy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pxyvlzei.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gjscbrjf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gbtafipo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzssnvja.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bacdebmm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jpusmlwn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hfjrwjdw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zevytjky.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3okbosopq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ifsfhknx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mklyvfhg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gemdrrdt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3enotsjtt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wplhtgoa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yfklnqjj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zevphipr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ympqooao.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qeqrrfvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3abeslkim.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iaktxnvo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lfsntwpc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3iijxiclc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mkftbvby.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3croqlvro.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rryfudkn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rnoeqitw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dgjzeoxy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swmocmul.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dnofpptt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pbzosxqz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jotshmdm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xtthiyzm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3crpijjgj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xluzksmk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3duijpeql.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vdejrzdk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ahernlzs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ymywrbpt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hjddlkiz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fmuttaqs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ojodobpk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jhixpiub.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3njawbehu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xsdauwxj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nlfjnyst.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3easaifru.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qkupcgjp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ruiewmlu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ttjyafhd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rvicnspn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sbzhfzbw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xjillwtz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pvhgtvzn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mzvtwtlx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ytkdwqga.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bezqlksb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3miqkxsyo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3esditqud.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3botjfndq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iabilpow.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cjjrdacx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wekjlafz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jcjyrhta.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rgopmjsn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oxsklyxn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kondislz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dqysjsdc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cpofsygf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zokbztjt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dictatye.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tfcyvval.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pgjzandi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3suuxmjoa.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vsgnuztg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xuoqipjk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fubaopob.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3psnolveh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ypoqfovw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3epyuyxbu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tfttdktx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3csspnqje.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zqqbtwpj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3natwybsu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cxlmftay.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3axbnrsdt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xcattnvh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3konnhqal.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jrjunzba.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ehkwxutt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ugxrmhtt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hqtgeafk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3smrrmsii.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dtrmmkgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jpycxafj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3docpagst.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ggyolqiu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rtpqxueu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tuhofzhp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hsmigrsd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rwbmpqbl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qralnvli.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vlrprqcs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohtxvadt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gxhgxsww.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ndgaxrrk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jqnarteo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3prnczqag.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tkhkwpfg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qrcrdffw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lfcygjzb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ltpohoox.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qzylajmn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ygzyugin.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uxhxkusq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cykpthee.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zpwqjxkm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zzlmncso.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3epdbpurp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hbdmbjla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmaoqxue.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3scfcznnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qamzbnin.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qfchegws.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vaodjlwp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cenxoexs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mvbsaqcw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3khmoyjvr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tsdczhre.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ybuqppiq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnbpkpsz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bclmktja.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xgmjjoml.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3febgeczf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3euylaulf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vanqqdlx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sukyhrma.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wmejoytt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bxadbmfc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmuhiiqm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3eyljvbjh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cjsmcmfb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zhdzvlln.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3clskhdjk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pomooprb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gvqyzrlb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rpqgnhmm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bubmtccj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzfamlj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fvuaisjm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3llbluraf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dhbipaaj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3trhryezt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sxvtnnly.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3perjlkfa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nradgknh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rqwfauuq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jaatvwlj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gtybyxgv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lcyznnat.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vkrtpynv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hinhwzmc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gprfmcuh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mwaolkrb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3atnjsdit.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cwmnzrxg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opbguzxc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3izicrufl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3silphyks.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3puoqvwth.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rilekgqa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fgqdwele.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pondanht.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lrsxcxlz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aufsiqcb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3doroenrx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kkgnqpkk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3irrrsyzh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzjblsq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3picdyzsd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3avtovolk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mislwhqq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cpyznhjq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gikgzwvw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vryaxjco.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3umpnxclx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sxuxtseo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vbghhfya.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hdjnoccg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jglpjprc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3skjrigda.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ilirnewk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oefzphrv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ruaufejm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zcgbpacw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hmkcwuif.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nbbivafr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hzjvldhv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mucopgvp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ajvfsmoa.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3niopujmz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qhivqyqd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kvsmpikj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3timqbbdd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3avjwienz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dzwauklj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cvjcatum.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uuvzmjoo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3etijtuio.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pjvpdkny.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djkfnolb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqqwtwea.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xgfdblws.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ifixewrq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwyaiqoe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sltlziws.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3onnpmdzd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bpwhuhmq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ridzitbg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3imbkdmsb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrfdiycj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pktxxabw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rqiitbtw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxdmlevw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhhfnxfx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3skepvpju.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qlojuhrj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucpazsjq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qkuiygpi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fzecuetu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3szqqhcts.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brqaxeci.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zszqrkmw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcuphqj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3muupaiqp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvkyxqj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zkepxqzz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lskshilo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bdzxzazn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3huhwhrhj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gusfmrom.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3akvcmriy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3awfacobe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3brmyfjqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwoewkod.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eaikqajo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auemacbj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mgkruxaf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pyspylah.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kevtevzm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ixvtgagp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fmowiopf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rhlaidbs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aanuflla.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wiitkkcu.html


<!-- 参考信息 -->