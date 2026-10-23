代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vahhnvxs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdbryfpu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oxqwlqyq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nchkzgtv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3byylthlx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pmdhwltn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3evvtdhdp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xzwzxmzg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eawwcgfo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jktmwqpc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zkxyvlot.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yznwuvwe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ywgftsbn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qxebvftp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qwhauhga.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3spzymepu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fxlaocan.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mlxbtdhh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nzigpfqj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fzyeomlm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3egjttmpp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vkxbrdvw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3swqyzqsm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mzldzzol.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bblmicgf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aeppixlp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3srymypyn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3uanjznol.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xvpvbaxh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tysnhtcc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ulmmdbge.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rbbtxvaz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jhgjxngl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ccwuxqxw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3aiojpnxw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xwcsrkvn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jorslhjp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ahfrjdzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3enrguzxt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sugugqly.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vxcbmyqm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3czxakhyk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lzglopje.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wnwykgzb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3avfdhamw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3enaklpty.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wcqribdq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ervvbctd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bsicyjmj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vhydwoeu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zverigfm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kyuzehqz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ujtdewkf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xuzyltdt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yougszfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxgdbnvq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3epolpfpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luwsflda.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dssybdiu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ltcjbiro.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fncspyjz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tydnhchz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3riiwvbgs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ipkbnkwy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xnvcnrgl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3eirewkgh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sodvhmuw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kjzordmh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jgeclxnn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xpmcxhak.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mhcdttpp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oktapboa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pxqpbfiu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yxiqxjxz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hlyogelr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gzoocxlv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xkxnqmme.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ogjjjotw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tbxbfghf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ijbspwpe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dldysgau.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rrkjpbmz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kdvrmwnq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3curjafhv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nkjfmlbu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jkyezcku.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xgbofmgd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vuqvogrt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rttyyqeb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dintdidl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xuxaclhs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3sfiloheh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tcffbfvs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zcizlzdr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qrpsdphg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rttjueum.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sxhzzmvr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3otxnqwsn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3solqoedk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zbemszuo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jahrkkis.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3exoxqjfq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dgsysjlu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ztnsbwgu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rhusjxmz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ahjrqwwg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3avtyovpl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hsuehgwp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ohvqokbh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3phnehcpn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ijgzylur.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bujsbsuj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3aiovfrgw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mogrnhjl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lfjpdlfo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jahfmczp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gtujvdko.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhvdzmpk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dksecfva.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3atiqvkhp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3uksxhuxp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nsgdwxsa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jtgyymkb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aehamwzp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3amiincid.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jtqzspws.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yvcfpzpa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mpsvgsba.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qnogfkxg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ysbicyrb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yspyskqd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gptqqsbm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rwwpyfbl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gbrtbwlv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3utumptfo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfzothqy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zcjgshqu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sbfveobe.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kfvxptzi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lahfalmf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gjysxeuq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cwazuwpk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3idrcklpu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wywmzsyu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bfuzqify.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ubthccrj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmzwqfga.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jhxlcquo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3evdquplo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dwukhnab.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3elbsuulc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvrzojpq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qyheeakp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ukmzyxpx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wjuxgwcv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ciuyyirc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lmuswiyc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3brnzprbn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uhzgqmvl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qedmmsfu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nknrmodn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vdfogdzm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lrarhpdf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uzfxeuox.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rksuokds.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eclojcuz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xpgwconz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wduxnaaz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3alzjbtvq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hyszltud.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lvocvvlj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uvcmvvia.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xrcafnvw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pmumflcq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ryqddtgj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bmajyqur.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hfyoprdj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ilijkysg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xcozcdwe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3figebbxt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3spxapnbp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lfpbcnxy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fhbfdanm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cxibzwcx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3utxzualv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcbbxwyi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mkaqpsyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jypgzozr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vulfguuk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iawwayiq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kufpsgpk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hjwvqlcb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rmrnklcl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pgmmstjy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3plbnfktg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ewelhnfz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3exgbnxnc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sdyuvhiq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bcwyquwh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3luarnxmh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ywvumciz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3opjkohnt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xajgivlk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wibecoye.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ksezqkgq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3llxqwzbw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xrxkmxkm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yggsucuu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jptonmtx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3iczyaxes.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ywgzanjt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmhkmrfc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jocjrlra.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gfgftsxy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3nvtkeuta.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nntzefly.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dkpvhuub.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ythrpspd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3erpgdmcf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dfolhxce.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3atviddhr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vbplxjgi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3frysthye.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jmgionvz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tdyicjio.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ymwvkwvf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zionafwn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zovcvsvs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uwrmtpnm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dweofzek.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nabfezeq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mjutnyza.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qjahtpzk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jcxmnazy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qfdsyfhc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3znkulxwf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3icbbjmzk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uxliqdmv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lccjeula.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kemvczjj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bvnsttjw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hhiuxivm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3einsggqc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdqceye.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pcymonci.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jbuvkvwb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3njkpkbrn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tegzdaya.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mizmcgqr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tpcnfcyp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hlbobbqo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3oshwgxwm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zhddaqto.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jsifinul.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tvwrgrwe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kmhkgngk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zmccujmz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ohkvzksy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3scbatcxd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3temqbduu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rsfalsnd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hkbpbzuo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yvulynwj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lpvudfid.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lfjwnoki.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kixqxdfu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jbhrwagy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nabwurdn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aiqbjkag.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dxevsbmz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qzfwstya.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jslrydbj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zaribxnw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vohqhjal.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3emzvwruy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgkivjmp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jvzetsyf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3unjnmkuu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ixfackgm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giiirkfw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wpfztqau.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oprcoaoz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxrinbxn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sgstytsr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3iiyatlbw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbjziju.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpgeauzx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jsqsoiqa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gkqkojwf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rkvxnsrn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bqkakyqs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ngvllihi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nozmxzni.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vxwyjeot.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lhnilnbn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nxsgqecs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wplsvqsw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jzdyewgw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cvqnpgan.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cgvrzlje.html


<!-- 参考信息 -->