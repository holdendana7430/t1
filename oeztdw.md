代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3usvfdkuz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3liucuzod.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fubqldol.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lrqibdoj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dzqrsaek.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rpenbaau.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3enrbjtbf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3cyyvrmwo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zxuhczvv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtgjthsq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3icmndljs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kdmjvtjq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3shkzuyjm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vkdzksiz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtppwna.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cbielnwi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vhyseqgh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3azorzrwm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3riquakvg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cmsghziw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjcldo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rbkowmje.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yksfzysv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3yggoborb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dshwgqwx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pqoqohjt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nezfhabu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3inhjkuuj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tsysaqys.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jzgoncsi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3niqujbxy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3idmnefbp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3afqlbhdy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jvyqntnh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vgrrifxl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zjsnwlha.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dutoiisk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3upcrsfyj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xkupomsf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lgmrokej.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bprfxzva.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3owyosfjb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3oknzezez.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rwvkcmzh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3aevzlagi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jdzdedpg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wbfrjbij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqrprfzg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ofdzkmul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eraseanx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzqilsqn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3poxmqyss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3opiycpbq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xrqfczpv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xuimqzhd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jcjrdflo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fdiunlva.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3faoguuzo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3omwaiyhi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pwgwepxq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3quxgcvod.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ivxejhaz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3szxvpejd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tksbokpv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qflbexdn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wstgrtmn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yqwjpmkg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qwymdicq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3avzniexc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pesyqurv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nuujeylz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpcvetbn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pnsntzwk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vsqgfgvb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ihqrpmco.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3irnaqrkr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pxuevdbm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zpylcvck.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uviilljd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tszoktvu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3juowxcwk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cofqtdno.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pmkvbxap.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3szmoxxye.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lcbrlfen.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jpqwsfag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ivksboyb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vhguzvvk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rcudjyjg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yujdplzu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3utxmwnrg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jlolewom.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jhynchmd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hknaxbpk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hntpyara.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uzetvrmo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dtdzeefz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yofwnpru.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jscnorft.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vlzdziec.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3haqxgrzw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3oaodttzo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3swyghqhm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fbyxxptz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bptrjpdc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hukocxdt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ztzpzonw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fqbobjsf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tqaamwup.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3illqdygr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qidciuzc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vstufppr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tumttamt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vitjcpbp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mvsavvzf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3klepjcpf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rdwqsdnr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbffjia.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mfcwmdgi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wlsuhqjo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3eeijdvih.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qnrvagxz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dqhgfyzv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tdhqeylg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jcydfrnq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqufpvsd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uvevjkzi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivdskncj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zlaqujof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3icltjngg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ifqtzwld.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uakhypba.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fodzhngo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sygpwlnw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ztlxyvyx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zuppcxzd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xokepcwf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehnygrdp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jelsfvdp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wfcqpnwc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bpfndbbo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ubthclqk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jmockjoz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3aegkbsof.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kfttgaij.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gjlkeqrp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jtzcceuj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owjjvyzd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkwmqxnf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hmwtuped.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sqhjcujr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3sjghzste.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3csdcaplg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ravbulex.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gognkrub.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3isufmequ.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vjzuhmnb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3agooqbrv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oabzjpqs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pijpurqp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qezcblrp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cqqozidq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3incangsm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lwauehcn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3opjwwbjg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pkriddqq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rvnkebjj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gbhlnwsw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuelbxcp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tjsqoviy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vjwhiuib.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yywtrikr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ikfykgje.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nlqsoxwh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lugljtcn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ulhlrvwo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fekuxngq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eiyaufvf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jwrlffdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tushbkel.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eefrovsv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vkfhznop.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nkauqrvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jrjpzyhq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3exqpqkzw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3axpxrxmf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iiroxfnl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ppmdmpye.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wypnqppd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bhridura.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wkcqptxr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iiexlgqk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kwflueyg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nodpnvrg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qsfqcfba.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3smgiuvze.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3diwgvqex.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3smtgpqbt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgkrudnv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yjmzzltg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jzqegzps.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nalpagrq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cmlazmyj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3novdinsd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fqbtwzkg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xncmgbkh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sadfmzit.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wgabdmtn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3glxasvvb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qurbxghj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qkewjxhf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3drixsiay.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xobrohdh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3efssqtkd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rwzqfeln.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ismgpwcb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tchrgqdw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zwdewlqz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3twctyfbj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iznbbnsd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dpivultm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3brebxqgq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3crvgmeso.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rqjcmjqt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsvdclay.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3urezoeeh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3irpgpcrg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3toswpfsl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qjghgtrh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hopxeinm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ccbiesny.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vlnaullw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rsekfybz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fixlmlct.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ygiurzvq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nylokfhb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ryufitly.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3inatfutn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3uyezgtef.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3khhforez.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yczpsupl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dzkgkbhx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kjkadkgs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrobytpz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3olyszpls.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3aohvnfbp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3palfwzfo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uwyiofqf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sbuysmpr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nmesejlt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfbrtoee.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xlpuisyw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oxnnkjil.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ofeogdjb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xpowamoq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bkwozmsm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uvuzibog.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dzuhawzv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3epuqodhz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dtltohwv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tsvndspk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cahxffxp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekjfrdss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tlwxvxtc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qwqwrrsz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kswzhxyi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zugufgzk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3serpxqjk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qcumrlga.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3itofcfaj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mazlhchd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubrjeues.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nkwfitcq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bicaeete.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oknfawea.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3btsyfhxe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wuwgazzh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhqcdacc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vcrkvqvy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gsblqevu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lgbivmcv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pgaqcekk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hzwxbcdw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pbaryqsx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3muxrcbbk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3znzygfck.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3neaxiujs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dhnmzqdw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rzexxwkc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3offrtuqy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xboejawv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ievqfxwc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfrprtp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gatnfosi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pejaptik.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3oxixudei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rmedmlws.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3njptstvm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oknylrqa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ycotfhkq.html


<!-- 参考信息 -->