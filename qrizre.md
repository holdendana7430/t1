代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yxcemudg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2imkwashp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gercdrdw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gmbpfomv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iqdwpujc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2igqhojtv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bsvhwzvq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uzllfbvh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zaiucbjx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxnbgxwt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kxqabcji.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2huwznrsy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uvadbatx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kouoflnw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2abyodwjr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sitywdnb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2negeogli.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ylfuadkh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nndastxy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xwmqwmjq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2taqyuhgj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hibruxqw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zcuzsmro.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jsuxqzvw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sbkydpyc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2itlexsqz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wnixldag.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pyrrzefx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aioafyug.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fjkhubsl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qunpmgtr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2uuhclofu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2viztedby.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wmopajbq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rwreqcry.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ipafuoqb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2neyalyki.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yepnnfdo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2otltihhr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2cqdaatwu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qqvaktvw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hgnrtwwr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lajvuxso.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2oabuibfo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bpldewde.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwheslja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xtkcyqdn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hqclubev.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bncsxsew.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2msvxkcex.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zddebtbh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nomhnuwc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ztxpqqsi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bnxazjlx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xvnergpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvumfjtn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nahrznon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udovbkxy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jrqyserx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pzyeerll.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbvfiolf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2woqblqdg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tkugblmy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wreiolqj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2tcostdlm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rjwafknp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2erhqwago.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yofhadnl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uesndtrh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ogjpxpmm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lomarjfb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pptygsuf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qvslihxv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mxbnevha.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pdzlhvro.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qroniabd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jxwybkuu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dhjtfnqb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xkwaegkz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dgofzedy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2webpwkyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bcdgbkyt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2amhmkntz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpqjbvdo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jaahxtjo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jyemyyug.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mzugafjh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lweopgpu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jlmfuoun.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ngxdavwv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xniupkej.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qvieakaf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vbyzvgfj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hzbpdzpn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ynthejve.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpyhecqq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zjzbokky.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pbqpselx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xpofipwr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rnwdbdts.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zfkfocgx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wbbjhdib.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zapzfcwn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2acmrsdvo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zjplgfgv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fxsktnmg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vlcyjfxz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qbdofndg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2creetngs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ovlbexes.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zuunhomu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zhwfzmix.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jzxmwkai.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ffikvnzm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbubsjfh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vkehxqcy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pyxjzrof.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qndrfrlp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vxwkcstf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vomgvwlt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jqbjyitx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fcoftlat.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2djvjbnjk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cmpdqeqs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zqqwopjs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anijkptt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qyqoufeg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jggrncku.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nurtxbsd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfyaxppk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tpvtzeyi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ouqwihjr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qumauzfb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dgdcctsx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2sbazzpsv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2psoawaws.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sqlognkd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nlnzzsyz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2owqscyva.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qdubwyjg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mvstffzn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ewxqjbfe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nlyoidmc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qkugyhbk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2adwplogf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cejspnxo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bniodzjp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cscyitjk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rjomhkdw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pfpavblb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2naxjaxnk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xwaahemz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sisraikv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kpzbszrs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2psobcboc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2drvwdfkj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dyrqvykr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tocnednk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtzmbpbn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ktdcislq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jpyzezvz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yhdbfmnz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nugaxaas.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nhwhxovf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2adtrfurt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rcfastrk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hutdtmum.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cmwlemwy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nifujbpq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bckbkfhx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2osghcagv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dbuxpvax.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnpavky.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2oscwewar.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wcghceoh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ioduvadr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2koetnprq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kdenhpdg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wrqckzaf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nwifnmla.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ewgqukbq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2njbjarrw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ebmmiarg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hsnzqapx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lvzwfmqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgrvaofo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zyurcars.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivbfivyj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mreomltv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wqwiynes.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gkxuteeu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gyorrmqn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gqhzqeew.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hqqhdaui.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ecsrfqec.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wtdbrziy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zbwmglqv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hkkpapvx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aguqkkmt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2thymrzkz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xyhumwcx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cmgcqbwt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tymkzkgp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhaynxq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zvflywri.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zbxbkqvo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dwyilssg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ornynisq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cwsghyjs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2emjwqjpj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gxqaezot.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zefivkjv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lfezksmt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvgoqcm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yrndpaiu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hilcwofw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2murcouzs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qqnfigth.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fzewaxaf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vxdgbiqe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sbuuaotn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lvmiskbk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gsccosmc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zirypydj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pwyexktc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2aazgszui.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yqkwsotf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qrncfmkl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dxxaiwti.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlivhsgm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2erfjyiap.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sdsyuvjb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfrrwbav.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2elyikoph.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gikouvco.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfehtvxv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gnogmidq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hlddqdse.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2crmcsohb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kxswhfkf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hayxjbff.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ouxflswd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ulnouapv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dpadorxi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2arvbfzxm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uvhnbzlc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wedcoijl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2okujweue.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zmbczfjp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lrmbkjdz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bakithgk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqewwsyd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ronbgnab.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kympakhy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gskmblrr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dsicftmd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2uolafwbz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mczmrmqp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2blvgkigw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fvkuqgoe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2akelywyz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zvlnglar.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hbekrtud.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cvyoycix.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2creztsvc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vexxketr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2khmrjllc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2aikazupy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lsqmgync.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hsxmqqtd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2opllhazi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhahfwba.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xkeomalo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mtyrmuff.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kgbhrlvz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeasjizd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qlkpytyr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lixzjdwg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nxmeblzi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpgacejm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uuksnrxi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrcxpkle.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vnyilgrx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2psmicoed.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zogcadaj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yfqsjwaj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djwimfmi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lramugwc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dwxxyczx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irvlbiag.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rtgyutbo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xmqkovni.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2esinevhu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dqfimidf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tsujkziz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lfajpghg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ejbkeaza.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cgpcardv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bffirqvu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2beeulrnx.html


<!-- 参考信息 -->