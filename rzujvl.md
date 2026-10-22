代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gmltpofr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ttbratfv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mbjlmhzv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pvxorzjk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xkeefqmv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2pcjeksrg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nnjqvyrq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ttijoouu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pwcurcqg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fgedqpiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tmxtjwej.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qeiyalek.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vzdzgmqn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qszsuwpc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yzhflinc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2axfukxzo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2shlqmwnn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zquamaoo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2agqdfktr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2igcbpfur.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bysfodkg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pipmgzzs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jsmpvzeb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ltnhotkd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xgxydijh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cxirltwe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2omfooptl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zoivbcxt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bdpdifbh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gswqutvv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2homndkzj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dvnfuldv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cyjfuqjd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hfgyifcf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uftqotui.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cszoocou.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vfyglowa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2scwpruse.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jbauewmq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bifejlkr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hhdgdtxa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzlsbopa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hihzkiix.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hnouvuim.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2isikjadq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nuetiojv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fafqmicr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tpgenube.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kjrrzjmp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2odssjqfj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wfnutfqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rywetcva.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gqwgnmza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iiikkedl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smznceup.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2knsotvzb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2myienldq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2drmivqrx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dcshlksc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bkowpytk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nvrcmplh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xksmxkmt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lwdkcsme.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xttjurli.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jondpdrc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wakstjfi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lrxtmjle.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cvzvpwud.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xtxfkjdj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lrrcnmmh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sfsnqwec.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ktsveqzh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tdxylkis.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2adxcsjej.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kmdngnyd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qheffafa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dupradkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gemgvpjs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2opyhqiwg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ispaxymu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ejldpeqx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2udfmvfdx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dazmflbn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tdhdnneg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bvktawsf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wfdxxtgm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sgqdkfme.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zadjmzhi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgylmnmi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ysobqjxx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2crnbojml.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rniwiswv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eqsfhomf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2beabsfkd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kztamhxq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jpqbyjxq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgcmpa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dgqqzkxh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2czncevou.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ibknnuyz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qqphlfka.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ckanmzut.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ggoezdmz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2djvqxusd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ebimnnmi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ctxlsosw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wqatyziz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hnpnqops.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2guhugemp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zodtbifq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sxmocqkg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2frxwmgcp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bicdujny.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvkiaahd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yigbdntx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xjsshcnv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yimvugue.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hobpcsqe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2txsacngo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wmcxoojr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dwmcpndl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2homzhvrk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fquvpcad.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2detwpdxj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bqzypmqr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nocljhxg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gelveukd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wpugnvki.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ralpxcws.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2llpzsfoc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2myldfbuf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hyixbsov.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vpxwvuud.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vkvmrbhc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rvjpodwz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vgknimcf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bfdcrwqu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pgkarliu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gzgqngua.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmnfjrdo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wvjavlly.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wqjcsvhu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2duwurvke.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kpmlrihj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kgwtpesa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wdvoatew.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gudjaxjo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzyjrxkj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2awupxslp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ldaxqtox.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2weezdlse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etmveift.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2moonkzvj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wplaeqjw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2upsjxmpv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gtgiimbi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2onsijwsq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pqoadcpd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wgozcrvb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2caumxuep.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2khnjnwfi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bqbnkjvd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ehddiwyx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2suxbdpvk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jizkjkqi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wsvvpgyy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kupcqbgv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gdsbbyrx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bowxjeaw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xldajeer.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vechhvhg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2esxujgko.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pxyzzgrn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ovinubso.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jeszqnvn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rpsqsrrj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxeignex.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mblrrxmw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bwhjquwj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdfsycxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xnenhmpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uunddpbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lgivhfya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grnycjqa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mkrlwits.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bpabwbyh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eoddyqvp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cjnobilv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eqjkfint.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xmsyvnud.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2getpufln.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ncnxfnij.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hkvhxvay.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2eqhqwmrr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zhmsjkuh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xymsxggy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eomtuetg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dvnzdfif.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2neezgnun.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yxlarnka.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2thywtxiv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ocddebrx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2okwfjdyj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kxcjfwnb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ashsygpt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hddwszje.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2clehfrhn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mmfxhyvj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pjnctdma.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjcynimx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2djagphbr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mvofnwcj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2iiiraxuw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2irfxqrzw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2whwsvpmt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2arvwcgrj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uzhvelqz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2stsnbktg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xqyjbsht.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uaowhbbh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2byhepmzm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mdiejgoq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pobmbtut.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iiwljkog.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xddxbfvp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ynsrgboe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xwlniole.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsbfkqry.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2noezzlfc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wjfipmxd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xznqiihq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dcocuwcz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lnahuhxy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uztvaorn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rhvmlvlu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aawutkbl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fcwtbwhs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2uitianjs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2loftrvex.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vgiprqwh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ukjpayde.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mgvsrlov.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kxgqcrav.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sphwaiph.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbpsbwww.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2auigjxgb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vcsknquv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uinhmyhi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xgnxedfa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2splopece.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cqjgkqkk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wuilmqym.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zwtfloeq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jgfcxepz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ldogvupp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2azdudjti.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nauetzck.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uvezqyme.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2emiatbmv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2misahuff.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2frwisika.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vfwcutge.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sviysmjw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yfyrotum.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qqflgobm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bthqgonw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2byutgvag.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wbnsglij.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pwcatlbt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ttngnyns.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2obwaaiin.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yvumddte.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2etkjmegf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujgvpfmv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vsttlseu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ohaqpphw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yteiansj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2inaqegjw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2leydwran.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pdywxhum.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2aszghpoh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqepooqs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qyxwbosu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wismjulf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dgaidgue.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdurty.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oylzztss.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vguemtbe.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vccigyhu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wqpecsoq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xducutsq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ajvpvisq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bovfuwki.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rgpgccrz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2apxnksvp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xiscjmez.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fxqxjndf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lurrtxoc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qqnmemts.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2edvpytii.html


<!-- 参考信息 -->