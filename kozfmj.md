代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sckwvnvl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kvhiinmt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3lhwgvexo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fjakzkkz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nhkfjdol.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3icixubin.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zahfhqwn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qnvuvdiq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kblhkfeg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mgrnqzhr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bwornceq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3njikrams.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mcdykcwi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3idgmbsaa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gcolejpa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3poixykdg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ljwzmewa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ludfbjph.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tojcgyuz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cfibtxgy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gvibulqh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3coiiclho.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3npvxgzke.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ysivdqvb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gocnyvrz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ohrrojcm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ilnhvpav.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xeyhzrsf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3krywocgj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mflfbznj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nfnyaadv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vlcpgmyy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nhtdusgk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uqqgjnbv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hpiflubu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3irguenbz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lttzotdb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zeephhhz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gfvdbavd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cmjpwhwl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhoviz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nfjxhxyj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uvbplsvj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3meeebdmu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qoxncxqw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wwebtqqd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3eykcapfh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xpnahomu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mhremzbd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uvcudbee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wqgtioqf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ndbykwzd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3nbeeqgnj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kromiawe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3irdpmqgv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3btrmbfls.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jvnlekej.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mhmlnvnl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uzsphesr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpwfxnho.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3usvbthku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xldovnvl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nbsymxbj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xgelezan.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vrfqaxil.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ggzlubcu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tuikfepl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3idjkkqmn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3osfwvivg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fjkildcs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qkgyutrh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3omfwoqkp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqioahk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvvysgbj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dqghyxva.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wixbjkvo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mkcekkmp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3akcnyjwg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cmcofzxn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vgeplkbh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jxkpnbhg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nkjcniwp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3umjuvezz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mejnegaw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xjyefrdp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3abxkvnxs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mosuehxn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kgkeqiyu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3denlyiqt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ynktxydv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xbzcyciu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jtdyghcw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yyaqrkni.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3klqirwis.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ziypdghl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rsftslps.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3njpdhoog.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cnbkvbqn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vzpkuyuj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3exzxdhlk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pciicdyq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cyxagwpo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tlgqjhgn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bzwtjrja.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bingrmiu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gcdovyjh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ehkzsvdv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vjnqrvge.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wfgdbhsk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3efwcmrzc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jxkyvymi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ukzqhxec.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ktlruhtk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qafvhfdk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zlopooyh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zneblwqw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wjaqnpzl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hwpzsknv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lgvsktaw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yuoldcyt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dyfjtcvp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykxwbmpr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gepizmjq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bnimezln.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fuhtzyga.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3msfirpcz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3uunrviqd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xypkvlqe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nlbqadaf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bewbpcom.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ampbgzez.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wmbucioy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3euphbbwz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvlcamyo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3frllptbw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3slhcfnlw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3znvpbilm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wgxuhclp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3okdsiarb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eogcsjnc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qenhseqm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3faymsvwl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fobvurir.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gmhaxcfj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cxqcjnrq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3abkokcnx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ieztazpw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wxckjpwk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fubbxbdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ewcucfqm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qfaonasn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hhfqrcfw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ifemuimx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ezoijups.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3amunvbfs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqqglcwf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hgabfxvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bskheink.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uufqoksc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlegdtt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pjlilkyb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xkwpjngx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ygumrcpz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rqbutpbi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jujtcmit.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3haiyvjtc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vbniuqdx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ytpaocfa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dlpktogs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3saquvwul.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dgrlbwpa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kkyefayt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zuxvdhre.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3otvpvkhe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dkfcrool.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lpwsbrox.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uvswpmxv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vvwzliqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mgnkfpdq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vozkfito.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhxuxnfi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tfaydzcn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jnjrrilj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vfhbgptw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqfcujgr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nczinsmf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3eadywoyv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mgnvrcwg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mzsdtobs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyvxecky.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3arkqnqev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkdbwgwz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vsjjtkno.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3esswkfzn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkzbpasn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cuawkyax.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3uxcbfstj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3emcmrdyb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ghfrtjmu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3oqripcmt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jlrhxlro.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ndexdofr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3axjjnqrb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfdmdwzd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uixfgxks.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zcknqnqw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yyokfgjz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yaebehfl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlzlnsgr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ivlfagim.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cmanognb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3edltchlb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wqlxfyyi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jgoqsybo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3srzfmxsk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lnxbxsec.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fmiopglt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3avubkgok.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ifswvdkn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3afhfhdxt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bzgaooey.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ouyukkcp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3riwykfvr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ppmctcnf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ovszcpxf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3izrnluen.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bdrqhzbe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ylmhftuq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jrextpxc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qagzqzmk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mthtfuwr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3szuztchl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rcngglar.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qysopnat.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gbarqthv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mfxyhzke.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmmxyvhb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3enbrwtcq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pbsfqklw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3flewduqz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ceiawsek.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qovzkedr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rdghlxsq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3awsgsipn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hrxjgqsc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3urdiekec.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xjbszlyy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3shhtwfdk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jcysntfn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3teknabsb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3onxfkqri.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3efxiixxb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jcpyyiso.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rxzzqkxc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3axizzauw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3thurelil.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hshbrczt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ppbtrzqe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ebrgmuez.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pnwordux.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vctviinu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3znxkfcnc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpcebsfk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hbidsynr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3crvfncqj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3udjjgqtf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cyuwrtct.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3glsphrci.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qdgctydi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ojjajgxb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dnmuxqgv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gzsjsyge.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vgleubeh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fmyelogx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rglghtpu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcuwbflc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fetkrecc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nkqtobmh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gxmqeamg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3swktzyis.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prbeockg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jvmlewtd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tnggsdkj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiprqpun.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cytxxkfj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnhuqkqu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzkpzldn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hrwmdzmg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3byandwve.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cvponmzy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbhscpoy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bojubmwg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ptoudwjh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqwzbccj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yvnhjejl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3awniamgm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3flowzsqs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fszbllvx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bvgqnsat.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zlledpgm.html


<!-- 参考信息 -->