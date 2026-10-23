代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ylcwofot.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iqszklqi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jiytbqvl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3giygxkww.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oagvviom.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzcyoyaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3npldekqd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nkyxawzr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cucvnoyh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tnyldqlt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ofwbecqd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lkdfgjlr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3clblvgdp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qtnxlyqh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gkafxzei.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ynhwllax.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dmurxnem.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zfnsuhze.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dqzduipq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3likbbxai.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mkoyehuu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cfkwptvn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ayttnpfu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uovumgbe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hbnwzolz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dlxbddib.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jcxobmvg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3uxkysnmj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wywuraio.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fnadzfrg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rbfrugmn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jokcwozd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ekhtmucf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3krbzvrxj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eldogthy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wpadxits.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ythlokdp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3sfemhjln.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pdxvgalk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hequfnur.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tpiairiy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gbemhuck.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mhctnflw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tgwbbxmn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ymwflgzz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pdcpxtay.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3drrhoeyl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mowjumhf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zolnwbdi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3orqmjvwk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3umwjqemw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkyqncnm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pbjyvqmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btcaugdg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pgchzimo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3oazazaqb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3uupudvve.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3burvnmmm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tmagtnvs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3echparem.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rkvdsugu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ebpxrrdn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tewwfgcs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3glaenykt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujankleu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cfuzfpoz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kovqrdli.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3adqiobeq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qaxltvsi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ncbilbvx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fkpkfswg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3szsrggox.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yzeukyou.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xjhfkfwe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tgalawgs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oisxqkwj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3udtucjgz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qzggmfcn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3byokecno.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nynzwbub.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dqzltjbk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ojempmyo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cmoipnkb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vthuhuhe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jcivhkxm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pmhitaqf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kkwcmzdl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cnuydwkv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wwozgftf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upjhbtri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bjybhtrb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wonspiso.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvehpbw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qvprizab.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ryzghotm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3huumfqdl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwtrvun.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3isblaegj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3befyecoy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hibqjoyc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ecwdyhjs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wptqztgw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wgobiqrk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kfbebflb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iuzevugl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3blvqgmpp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kjpcnyio.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rlixxkee.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xfjfhrqo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jfkvsjfy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lyvvnukk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jsnybfsz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wpcqlrcc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rrxspwfj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pkpptafh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3shmqqkzu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mtaijrxh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3evlgbwqv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3odemcsym.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iawdqyuu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qbfipcxs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mrejasuc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uvlizpel.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vypbkhrs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3noohfdae.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kplarlyy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kxnwvsjs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxhxrauc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ovrwubff.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sgahnkhl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yeelpuis.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qhzrsscd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xlbafvwu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xgnkkrdz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3guiatsno.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3afvqrdci.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nkwzdyfn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dqstsmta.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gqzzvcap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dwlwvdhn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qdzbcfor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hygbldgx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3kgrobren.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pttjtxdx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ntqlcupo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ggvytjqd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3psadhgrx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cydrptii.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3rmcadain.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xcigwayw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ybisgixe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfdlkwck.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ylrcligm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tpnznrhn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3twpusznw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3urhybona.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ufttewfn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwywgcyj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fzvayaxr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gxhznbye.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rpdiqdju.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jdefbloc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iuxdrvoa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fovhvzlx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pwditzqj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mgqhiims.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mephhjic.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cxzakqiq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dyfjwljc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kbulmsqf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ihpzmeds.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3klvacozt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpqneatv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3txynwidf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ktwghwwt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pceyxtxk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3legwcqrj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gfzbslhj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jylvzexq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ogojfopv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hexpqkal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weourhyy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lgxfompb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcmvtlsv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jgoowttl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3donwvsef.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fnacdgea.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kjlwadyo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hnodhwoc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vlfxsjxb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ywnbatxk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wusfhoge.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ndhuixkf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3elmbuafp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yoeyjlou.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wdecvcwa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kxarsudd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kljrakgm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kueutneb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cneyroig.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ryhtkaut.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jxcldqzr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xanwlnsw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3irrrjwdq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bhoziide.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ccrqqxyn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3grivhrtg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yhnbqtwe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nrhstmou.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfsuxcxz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kcavmuej.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wentnssa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3oumxrawz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jayyccxb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hhehjmll.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qsnhbsvr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3twbtynet.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rltjpwne.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jivysjlk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yyvaykhm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jxupkfho.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3fgumtqzv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qvrqtjnd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tclkjzqq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dooeipyv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lhlpmplx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yzqtpdka.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uqralkhh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3agjfkbon.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gqtdvyyc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rbyzuror.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvlwiai.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hhxivior.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3puviufvn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ooiqdkdh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ktqpvfad.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xvfoesmp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pomsnjwq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3chcytwvl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kjzjtvno.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mkgfgmnj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zfvzgyuw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kornbuqa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qmyuwqsq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ogvbxajx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dsfyugwc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fbdtqino.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jqkihjox.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nszygpci.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3aujxvhhq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yjwyjxgt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ganzjbhm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3grxmdddp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofratawe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pkzrkmaa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ouswkozv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sznfpjki.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vwvpnyxp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wvwlfxjb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qtembswa.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yrfncklw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3borgyxdj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bvzmzkdg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3myxcjsdd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sekltfhj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqhudu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vpzjvzkl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hvsnxlxb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3anytrkgn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mqibolnr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bmbpoeht.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ipjnqkhm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jugznhyd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dhumamcb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dguanwfu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3auxxomwj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qfcaczoi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vlwjojxz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3buibzgzo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dyhnxofo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffzduzwv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zrpbwmta.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dmeqwwsa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3azrzosrf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zemodwdm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ssqjaoba.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mvdklnkk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkbrrewm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qblnelke.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3phgelkxs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wfsteqcc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fxpabjxd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bohswvvu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aqdzkhki.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oetxkyum.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dhomuuah.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lxwvtwcg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vnvjtvyu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wcajeqbl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3emsbrnai.html


<!-- 参考信息 -->