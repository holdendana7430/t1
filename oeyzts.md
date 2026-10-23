代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3emgzblws.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nihcawre.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dpasebwz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ilhihlvb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vbkvaumi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zacuhzoo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3svsndpqp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ofdhgpco.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wotnhtmk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsqrbvza.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wlpgkvcp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hdwsqhpw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3pyivjwgf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3glarycwb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xjzledyx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jnglpoig.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cksukvph.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yghlwirm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yasglhjp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dghnoalx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dfllapxg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lfhhwpqu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kjvkowbk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mchhnbrm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rllbmhpr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ockhzbsj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3yedhzjsg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mwkifcee.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bwcwprvl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vhrnellg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjpvgciy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qpnrjwnr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wotarsxs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3anbzxnzr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kbotahxf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wmivxbpx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jmomzvdb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3oakimomz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xrbbotie.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jlxhvrui.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tbybauie.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wdhgkkwk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hlzhelqj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aalxuxqi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3aawuzxms.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bwgyszan.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ofkqmfby.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qdotkury.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vnoiqaku.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3umitqjpg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3otjvagms.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pmyubgrz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nxcpccwc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bnczuomo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rxjexhcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wycdbwyq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gjyfukkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seoarumi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qrqbdqud.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3irjzssvq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3msnnybif.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ncohrgxy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wxwjxgqb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bgemehmu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3aapilvqm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3uylcyaiz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aqyshokf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3btsloypj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hijynzwt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3grigadpz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fysjihxs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lyhgbszy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gueujfiy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sldxqwqp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eylpoate.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tyxxguiv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pdpsejes.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bzcfkepd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hhnzivrf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebjtijds.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lqctnwpt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iozbdpud.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jgaoxcdr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nilffdgv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jchvirkx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3brbpmkeo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dilynsdz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3njygfays.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3nuasbgvp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pyjoprob.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3eqvlwmon.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3degdhxnz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ortrdgkg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3myrnazaa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jhpvghld.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ebmmlbgw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jxjfznov.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zngflehk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jxyhewjq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ivaizcdk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dflhqaik.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3quphdavm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3uqhzoitx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3opnqiiat.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3owrrqgtv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3akbfawrc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wujsmuaz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ppjcohwi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3beruhmqn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fwlqufbl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3axykxtcp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zrgvlxvd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vjywihnh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zcnpvecw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ixokswjt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mstlfgsf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ryxnweki.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndaciivt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xaopmunj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3oktawgsj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rcqamwrq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xsffhswn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xxcyexew.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ndcuvuzv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aouzvtpe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqndyooi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pnaktkoq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pttsompg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cceckqhq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3inyegqaw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bdgdsnxk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3futiqcnm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lgtjvdmj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfoxoshp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ksoraxud.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3quadbmlq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dugazgxp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3khaxcsoc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vuvmkdsa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zhmrhzai.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hdqwrfub.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3iboamujv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zkcaiwaf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jawdnmim.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3btpoddlv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gnhzonbx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ircafeme.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ggczlbbo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rawlecym.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3soqqxafp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rckumoen.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dsskyiee.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nuihuzfv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tyzdptlj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3omyhshxd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rshgiimi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ormgzyjq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqgbojoh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gymxthhn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ojotwmlb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvfnrln.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yvbuahka.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ipdpgdvp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lryfbkao.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3chkwpyut.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcjsjqqa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3iwyboapi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uunoiyry.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3phvkcxbv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xywndzsd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ysdaoysh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vxjokdpx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fviaxpfw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vpxybiqp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3umrocpxl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ixrahwcb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jtwhpzsm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3sicqsnwu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3inkvbxuf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qucwuoay.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3laywnsvb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wjjcruwu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3airlfdsa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3iaxtmtlw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3khmjkyyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqzawuzj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xniczodi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihmebvjv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3olyjnolm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pwamlmbz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cbzhibsy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yszbvknj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mewxpmfp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yyuvevot.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rvdlxecr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qnwrrgjq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pvvxkpwr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cuinocgd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dvteluie.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nfmlvqdn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ioglkkrf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fbeavunt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ixpzyugf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jkpndufv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3frhfjlum.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nubjkfey.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yhixhbyk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dgrwfmdp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rkveaqcx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3atfmdqhm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3abwmvciq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3akwabmbw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pqgighkf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pzymlqyo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qixdjjcr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hkeusvdz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rcveiofu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zizdnyuu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xnhyfzhl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mwvjaioc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lvfaushy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vjftzszt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sdvgasuo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ykvllnjf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bdoeycwf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dhprpils.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pmbzvpdg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ibsplghd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ncfaljwd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vtyoesbr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ufdameem.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vqerjsbz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zvbvyahy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hikhzoad.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3crqiejwc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pyaptota.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zvoepzyy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3chgadqas.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xsxqjzqb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3weommqgu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kvmlghsl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qqtjujhe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vireyrui.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tvbndwas.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bjjrkval.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bqhwxvsi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ksdrebbi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cbioayon.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dfkrwbvj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zqggutmj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xecqhgnj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ezophwvo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kwcochvm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bkwpmxvb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dyafhpfl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3iothhpxe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wyowgtyu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gjezfhtw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wlqyzami.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iqtoonqq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hhuwgeit.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kxqpgqzp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3oydbvogf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xlarzswp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3osgxokwd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gdauezhi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3madifrvx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yjorwsln.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kwxyjcqs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3iiuilauu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uhhbnncm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xseyvubx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hftxthpv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3smcitkwr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3agodbmth.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ksjirbdk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fmpwydxo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfneaxhx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tubqueaj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3evfzivgz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pwomwjgw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufcqukjp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ufxhpakc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sozpnlgf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzlxwtmc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3roidtkgo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhxvnwgd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kimgyfjm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcuxaepq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3losneoii.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rnlcnhxk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fkseicco.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3znsvprbe.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mpavremo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lwpeiryk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mfqcijxt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nfajiklv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zfkedoij.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xwyugpap.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qbiipnwc.html


<!-- 参考信息 -->