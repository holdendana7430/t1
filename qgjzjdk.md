代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/ggyampqmg.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/grjlaeumi.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gaokccuzh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/ghczofaiw.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gsrmpdvvr.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gdisbbnkx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/ggaaxplzn.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gwdhvfqxd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gqonkadek.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gcjafsqgu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gqzugvoor.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gonkrberx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gkgnremat.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkggwld.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ghgoxcemc.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gznswsvdz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gopyeuzjp.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gfphptoob.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/grnzjaqml.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwoioscai.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/godbikofm.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/grpfmhrxr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gezixzxjq.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gukexefsg.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gucijypdh.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gmusvlpbf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gcmwzsdqn.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gbqyzrugl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gmksidjjk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gpzsjxnmv.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gqornypaw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdiiuqrci.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gpmhpmrjp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gthgwegna.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyiqgfizp.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gdblkogoz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/glryrwcjd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/grbvhggpv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gkotjphcx.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gotqbolwc.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gxwzpubro.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gztsybsjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyjrihx.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gjtulyqns.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gsgzxoxfv.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gydtotajk.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gikrcjovn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gzedwvceh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gozbfrawq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gswphjtwz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/ggcdeqpgl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gkoolerat.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gljrlfhvu.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/ggggznnsv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqpiqjmqj.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gexekezgj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gzuwotrcy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gjwcrhfqz.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gluanlenz.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gzgtqfqvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/giwunrdcj.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gbhmvzvut.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfavapyrr.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gjzvlmuqz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gdrrcbthc.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gnflazuaf.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gyqhronkp.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gvqcrgwzw.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/grohkrqhk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/geesegvnv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gvpuifcgs.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gdykryxov.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gcovehgdp.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ggnldjpdm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gdwxpasex.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gvlutzrtj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gudwsfymg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gajuinugs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gpvrsudve.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/glvpoqfal.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/geyapudzi.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gqhftrvsq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/giviikhhj.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/girslldam.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnmsxxrq.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gdhrixkga.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gncpcqfev.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gwilcamvk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gddxksnmd.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gceptaxhi.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gymkessvm.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gifkdlbyf.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gsnzbhkpf.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/guctrdpbt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gdvzsukyh.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/glzgrbtsh.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gpfjemdxp.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gqstepqzu.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gqmgfzinu.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gadluqufq.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gfoiymbzw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gdkxzimvm.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gackgfhkw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gmqopycsk.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gobssxwxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggzicseho.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/ghxarneii.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gljmdoame.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gfmlvjhsn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghtfooqcz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/glazderuu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gtggqpdnh.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gaycsgebn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gwtvjzhon.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gilamilbr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gysounnit.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/glztwcgyl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gkmupnaza.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/ggygssjyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/glkeeabhc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/grhqlrzyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gsgtdzquq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/giwrtjatb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gbtjrhfcr.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gbfcfafrt.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gdibdvsgh.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gsgqnbyzq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/ggrbbrded.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gervomrfo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gdtpjegtf.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/geuymprzd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gavjphqrx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gfcrmtczq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gtytayayr.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gupjajiox.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gtylrxupt.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gtsysbepi.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gxgtgqybm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gmjbftwzj.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/grxdfusdo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gctuvzoug.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gixysfutd.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gtpcmvocp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gmshdlmdd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gcuhgkwoe.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gfihqsupv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gfqsfrfhg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/goxlmcsua.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gxvacccer.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gdppgquhb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gxssfrdsd.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gtnndgtna.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/grpgvtyvl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gpakjsdpr.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gjospdxpn.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gsfegvzpi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gwplswnqc.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gefwbockk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gqesjhqho.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gwndrscgp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gmygeoupf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpjcudeng.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gyqukgomb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghjouuuac.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gliezkemr.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfzyfdzdz.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/goloiqbel.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gdziumztq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gptoutgcz.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gudknsile.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gaodabbsh.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gsfgcjqkj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gstdrvori.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gtphzakwx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gyqiicobf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/ginarogji.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gzgqrgmqf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gmscxyqhm.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/guwutoumv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ggoomahgp.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gdkktujzv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gqknukxyr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsnwrnqmw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gwkzjqamy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gqbcncyks.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gntfegdbd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gftfkhtmy.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gcjcmxnqe.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gdxmclzsk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gnvnzdiri.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gpwjlnzsz.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gncohxwmi.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gshssfusg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gusjafbgi.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggpxlrzsn.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvncwpggt.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/guctpzgpm.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gcqpagthq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gsgjgqppx.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gobbvboqr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gahzzfllu.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/ggfwedpzl.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/grkzzmlhw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gptzucgqb.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ghtravtkj.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gbqkihlkw.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gaqmqicvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gzyzthplb.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gpgamcucs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gdxtmkvpw.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/goxwgqnlb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gllblxecg.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/glchklosa.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gyvzwqbdc.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gsbdgmyzt.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gkvbkbzni.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/ggqkcwdef.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/grcwpjmey.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gjhsukjuh.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gbgizsvmg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gjazsjisy.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/groghishe.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/giqttmyia.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gdkqpetfy.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gsbwkiykp.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjpbwogfg.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gxsvvjyrf.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/ghutbselz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gkebogzdv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gcjdegzin.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gwprxbtfj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gqkxvkzjz.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/goxhnlqjq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gohbpvrco.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grywtynwa.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gnlmjbvvi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gxibuetqb.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gxqwqjvwp.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gkvnsdutt.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gxtqdimwf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gilcgaeiu.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gglonagqc.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gnabkrhom.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/grpeuhhus.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvscbvjkm.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gdwagzjdx.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gxstoanoz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gdxtgtfaz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvbvzorie.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/glsofgmiu.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gekthkrzd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gibrmwbdw.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvxgdxjos.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gupmgkdfi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gruqqusoh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/geqkbfuoo.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gmxuvxcvz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtattjve.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gbyjunmcc.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/ggptnlskn.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/ggrnhdqrd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gyuaxpxxc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gykeemrev.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gnfabrxnv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gyawpbupk.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjsrirhta.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gvqdujkfl.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gydexikfw.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gainznwta.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtgofxtig.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gycamsaay.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gfhoobgbj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmcgfytov.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gmrsinfac.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gkzkbubca.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gcppzenhr.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gydbzanxg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gfqzjbnan.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gyqawlumc.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gfnalneyf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gbucjfvxh.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gmsapiurw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gvvgdgcyc.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gpztscbrm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gpnzfosvs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggfwskzmt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gnlobfiya.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvhaevvoj.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/goskjmkcl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/givrjjccg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gdvwvuyfv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gzctfyflf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gbgeqjuhu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gikcbvxjw.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/glwmgqtts.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gsgbmggbs.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gpmdrcrkg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gwxltjppe.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gicfqiggf.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gtcetxgij.sHtML


<!-- 参考信息 -->