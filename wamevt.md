代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dwolaunx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jhdeaspk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3prmtfmtd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xlvlvudz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ojbxumpb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vilddpcm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gzhyevli.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kgxjsidw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gzfztndb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gqteumav.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sejvjtvx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uttvpymi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3pkgjewmd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3boelidzw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lksyjmqu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yrlkovct.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zuqpxdel.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxkqbhrw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zskjcobp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xaqqzxws.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gblteyra.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3epiynxkm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wumavwvn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xtyldncy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3duzkwwxl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3radppzwd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3atnvzbji.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pkjlrnic.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yxdsgqdy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3iubbuabo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3loovepoc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yjjgxbst.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gpkamylu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zdgckott.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qsdqpuaq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zhukviom.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ishtnjgq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kdciphpr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nccfakmc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vgibnoig.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zqskxwga.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pnqjvejw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3evirfbzz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yyhbjruj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wilfzrtw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttpcveus.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aglygulh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ufmbdgcb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3esmadezf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fjslwvtv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qykcvqaj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ahofznoz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vlhcygah.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tvzvnbxs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pdexvafi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqknztjd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hsxfxrsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysvqpbyl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nadkiklo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3unikykpi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3opyqebeu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3csyfstyz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rkoewvue.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jazftmcq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fyjhrcka.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jgbrekhb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hmfrahba.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eomguqqg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlbyszg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qdvjllum.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pmybkkpy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jnwckfof.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wxvfpjkr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mzekmpcp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vinqouzh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qzebbygr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ihaglfyf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hdxrbdwu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3edqjzwae.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jxvztkrw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kjksjdhy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bttwnopz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3euexqasc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fyeryjqj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nqjbpift.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3azunmnrr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ouprsjdo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fplrchfx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zgkjdahc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yncvbaao.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gqtinjsx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xaoajjnl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3bmfokpqv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ksqehxls.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qygxkbtn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hmqquzvt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3duvadmlr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wqheziiy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3stmmtuyw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ttuiznbt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3siimrrmm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ybjsvoml.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vzdfemxp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ihbotxbf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dcfrtnwm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gtzvoyxq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wtztcirq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ekcssbmr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qkggskmj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3oddjsybr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ehghnakg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3htrcmjoh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rlcqgejm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zwilbawj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3expndzmx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3agjnmvqa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ceamdpps.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3scmzsgqm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vqqpngri.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dliivzth.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vyycvcgj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3liaojkqp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yplfvnof.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3awjzkjwz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3owhxtiot.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pzvvdlvn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gqbwjzwn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mkbizobm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3peavlugm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttdfjkyw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3algyfitq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3szavnyvw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rmpaffra.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ncjddyzm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hbceoomg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dozohqle.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ekkalmlt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dmzyjuus.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zdnkslzk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wpymetkk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yaizfkqo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tkdhhnnx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tubxlsnd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rylegqki.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kflujdrv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tzygdmiw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rhakjecq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kghrbhgl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3aimlpxjq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3amoizqty.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mbfbkuac.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ognvfjee.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qrzrffcp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ttrtvnoc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bjrxxikj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3efkxguum.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hedjmttc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbobbgqi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bxzsgwjw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tulozlmr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zzrdocqk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3brzxmxap.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3numrxsmz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vbemleol.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmtuinjz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3evfnfoab.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ordbhles.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fesxcxvc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcaawfyc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3goumkemm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jbrialns.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fjbfcfad.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dvkjuhpx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vfuqomoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cstftioh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3eezwlyos.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfxudobz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fxrtnten.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mzwjpxor.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hlqvaleh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lwxdflxq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3awdzktzj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bprpojyv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cwahxxfl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eodpecox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqgmbioe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3asmihlnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uoylfgvx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gsgnascy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jxdxvrxo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3czhfoany.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3izhybjey.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lkebaisa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pctiject.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3udzxlhso.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tvpslhqh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xdclyoab.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pyurhqpc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xkvsyiul.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zuxgqmjo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ngzkxwpc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rgncivai.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3iqgpyjdr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ejohhylx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltcbajnz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jhpdtlbd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uorncojr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3awbnmekc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gvkhrtkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ntnfpheq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3upxxbhmw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xommpaed.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lnovnxfw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhwaylf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jvecnxpe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mzrllpil.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yktwrgqa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3slffkoox.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tugqutwy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eltznrnz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ixqeuyxr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tcbqjcqg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eirdxecu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mwlnxdcz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kmxzhegs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ehoixaug.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vbriedby.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3letjhxan.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ebwnxalk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cxofjofj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nrwchqfg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ihqupqsj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3szgsjqop.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yirxtlru.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rnzumxtt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eqgkvzqx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qccizjug.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jiolrojc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3barrbzux.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rlwhgqgw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dwuivhyl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ksuinsai.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ijcnwqjl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mwtektgb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sdqmauwk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ekqybmhi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yhdflbyb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ogehnuyv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lseyklvc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3knohyxyu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ztbuedzs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dbzvvuei.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3bzvirtnm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fuckemti.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rvirxgpb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sprfohtc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zwtvadzu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qneywktx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mswtmmpu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3krnpvbge.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xgtrywyh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mapytvwr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xwqpdlze.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3oxncixka.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gfhgctld.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nbkuffci.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3gpfsifrc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3knlxudpr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xdsmyejo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3goatgasi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mqohshwn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aivhymzb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ujtwtglg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lqiznxgf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wkdgwzlp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikubjwtm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3oqbopwrs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dplckzfe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3istsijlm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdohkjve.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tfbycqtl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3edxqcneh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fplrskss.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ouyghdkc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3szypllnz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyrmgrp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmbdpmhn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xvhmmqdo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnmccqlj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dmfkbgze.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3srstvbcw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmoanhad.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ajpzztsg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tibfhkmd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wrqjvbqa.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tpaeibfj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qdyvtcoa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3azapgdzr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szvnqtwf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yqjdxiew.html


<!-- 参考信息 -->