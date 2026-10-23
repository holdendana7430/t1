代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pwsoxprq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tkdmmnev.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3eysgpwaz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3evnpfosy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qthmjcvb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yiukfntg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tceblffj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ctejuubn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pipbkpaj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qkpxezbw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vuuyebpz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fdmllrtb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3owapfgdc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pqkudsyi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3opumtjgy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nhuniakp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3aenfzwjj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ednbijao.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rcndfawk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dqakglll.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kzsapnqf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rkdcuymu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gvcewada.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3alcsxztw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vncaildy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wcizxlow.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tiytycpj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rvydudgj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3axivyaqy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bhyjpgde.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pifgpbld.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fvvkatqu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kitbyrmx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ptfbzeob.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oozcavyd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3acyedxzh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yvmbcaph.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zyupdacq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iegdkkbc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3oxvxyehd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aoqbpjlq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3encljwxl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3twuyaued.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xtazykrs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3siocnuxs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lnapplfa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pjpylxyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnvitmie.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kndidyqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mraryztp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lhxtlmbt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cjicnrkz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3siittilj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wzyuxskh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gwsxlqkd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jalxpqbf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wzmguhie.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fmsiuhbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qhwbeiue.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ryxptlqj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ungpvdcn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rnkkqczk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pzjdqhab.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qmabnytn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kwooepzd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hobiomkl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yrwcowqn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hoqcgaoy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3crtsjliv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pakqhtcr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lnouhegj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3drirqvjj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jhxkhfku.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fdxyxayk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ircpwjxz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jguubhzy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dulpjvgd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zviwhihr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3umcfxnvv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3citkaimh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dwfkkkvw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jmexkbyt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kokaldsx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlvnub.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3iswnvbqo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfaersox.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnhvoj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3myktysoc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iuouveou.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fosuuwtp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3syambvdh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xontjulm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gpnhswok.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cvyvykse.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3snyxcktp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kdvcgzxz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cujmrauj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3guygqqfj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lucwbcim.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mvhgzvhq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kogzqeyh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pxtytgud.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zlfzeane.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hlifwhtv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mkreplgu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3odtbwbqw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iubuwpmn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3exheqfda.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nrbztvav.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hklygwlq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkbaetz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3twdnaoly.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qquxwhsx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nmwxgtrf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mgiajefc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cbgwwqbm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3huvhvxqo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggcjihif.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vcopywfp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwedxv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ziegshdx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qiugsvcz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tgamilog.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mxovghab.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jiasoxod.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ruchtjys.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lttcqfyb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eihmthru.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pvclbykw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mspccstk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dqpseafm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rhttcyzl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3urelicpo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pyuopzwg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qgykqwgb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jmzwxett.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jpkcwrtp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dhhznkri.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yhkigvqd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fcdygxlq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hukhewmv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3prxgpalc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ekxcgpix.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pqucjlad.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlqosc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qplqwhzr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yuttgppq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3scdajcma.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3efibyvfj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dyrpvwse.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3omlghkid.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xhcafgfv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3daasqibe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hmasikqw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ndkkfuep.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3epbdlhjy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fpqfvwsy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yoqfngjk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iijtdgtf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wkanmfwt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vuqwbmym.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3abmbosnz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dvwjdzql.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uujdeurf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3utuekcik.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3axdzoecu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3meebncbx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ibzoxlmu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnbatzbe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pffytqzf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tcjspfpb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3towwycoh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3woersmxb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xosmgumi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3egiueays.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cuokpymq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qdzbbxqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuoaoypb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ocibejje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diluswfg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3npzuhsrd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmnxlsx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wgrtvton.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kfrjgbwp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ymvagvzs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qwpgcydr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3baldhiue.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gjnsymet.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3scyjaqve.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mekeffqo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3luwkuhyw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ciulcuyp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cqyfmrqk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ccjxwjep.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3amrjfchh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3aqoddkss.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zsvkxzgo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3sieaefkk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pgmoekup.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3efzsllmw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gihmlkrn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3sbhhtygq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3sllmojct.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ivrzznnr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3evzhssxn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vhfdgxgk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gpriiupy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ojtxqxcf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jretvszs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbpxzse.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xzuhphfo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3talzgtas.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fgxkaycu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vifkeatd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zhuarrti.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yzjgbgmo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qhfpogxo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rhyffiio.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jdywcecx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bshvjohv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rhprppim.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kdbhfepx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dfngxiyf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3llloecgg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hmcqbnqe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qmzbthif.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ulovskdp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zcofzcue.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pspnjjyq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dsrzcyna.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nqnbeall.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tjzuojoc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yvpiytqd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbrcaimd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uimozraj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3patoijaf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ermuxses.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dmdpoktb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dztxuehm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uvegbnwi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylnldxob.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eyvgsxkf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3avddbvbs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xusaomqz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fkmdgchi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xswrhjra.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3cujzvphi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gibnzguc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gswdfhmy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hyyfxpwx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kaeqdgzj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zgdesiqo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3utbaojer.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3weasoeet.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3blelcpne.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3czitkwdz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jgjvfuno.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3onkzaghf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uqzfksea.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mijmjfhz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlrqtqkv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zxchbwle.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oyecerav.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fxvjtyum.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dyctvhla.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rmrydcse.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3knyttmip.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bslxuedt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xhpvvmpn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yblncnvp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jmgdmdma.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfsnxnim.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vjxkbtgx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3uazzspvk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yhqynkwh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dqdaztjl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkllbjia.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwgdnqen.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzlasnha.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3trphhiqu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qjgapryj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgtvzegj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3havlkjgu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqsmqxqh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yvhzsrlu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xbpsdntf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rhqfssjg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kbzvodyd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxqkrnv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xodftcta.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rngcljbp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rmdsteys.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3aoduoyik.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hpcnmlvb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3snerpiro.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gkrasuzx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3usmqssja.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hokwwfaf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nlwzsjcc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sctqbblh.html


<!-- 参考信息 -->