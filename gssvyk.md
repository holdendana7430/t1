代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fjowazot.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rjmyxuvf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ceynlipv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2awqywhaj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fvhabcfy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2prgethov.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hmzhkrck.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2omtmzvlw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2itckbdbv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tjgswcuq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ooemlqie.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gthipxxd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2imtamrkv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tlrbmxlo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ncwxlgwx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ffgtssko.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jlqpydao.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2brvopknr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fsssuigu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cdkorokj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hrsesmmu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pfaygixz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnccanl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2anlzento.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2pkadnkpl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rffytulv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2caqnsocz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2amzsvlnk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wigauuue.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ettsmdcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vwbwtdhg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bygauqyb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jdznnnhv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2slmkcqox.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qowpgrhv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tijuhmti.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tvsuwpjr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ttddfzer.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwyjegia.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vsqksvnt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dwhptwst.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dilosltl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2otycovxm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rlkbbxng.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zpkgozcm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cudcmmbn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2juwunbji.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gzkqusyn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qtgwyvrp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dlkxefyx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ekppxlpa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zqhlowpe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tpralzrk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2apvrlbjz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2coyqdovn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbmumvaj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hlaqlhof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibzbekga.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xukybwws.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2pjiiusmz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gykksywi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jhymralg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hiamorat.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2abuxtwoy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gtwlzmgv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mbxkrotu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hnosklob.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xubnogzo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2opeenwht.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2efeekxnz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2glhihoou.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lklgltja.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hpddmygm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mpqbehnl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qyguyjis.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cekzplgz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uvoalmvb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cvewdaue.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wxxjuqdn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjkodxnp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2brfmnskj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2twgeoygh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nutsuykk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ortxxrhs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bepmcrht.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vcecpnsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cnmyxxrl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gqljenev.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mxkdlfuy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cooybfmu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xkehniah.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uhsgkqrv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rnfsrcst.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjonrenz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qalggwfi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vodojcux.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rsijomyf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mftizyeq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uyyxvfjr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wxrxqscf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kvwmxwuj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ysnzymzf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2acxekufz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2piihvizn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zmaehjaf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pgjkrxfg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vzsclrbf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ysonydqv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kujaaetl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pbgwpbcc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zngwzfbq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nxiorxfm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zbaxmcbg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2arsjrsph.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wbextkbv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tatlxtsg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hawvdnbn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2csoidkmz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hreqzzxh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uekbejbc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2udnaqdyd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oktomddw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2loijmdkr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tqcisujl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rdssfzmi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyeerrmg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gguabasi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ylavtetd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2urjzsxjv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oidfvmxs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2pvoxbkdy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tfkjvrlr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dfbftwyt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pelynepw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gbpkijzq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fhuekhog.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2oozjgwgh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjsbtfun.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kpkqqbmk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2havyiaqn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tgkqzcob.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zfebsnto.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2odnjfwmb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xmapasja.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nekdrpoj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ojtjxhhr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dyjwudbt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fbjgvdyr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ryugkllt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yehitibr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uzcldvms.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2apwxowjt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fvpmyjeu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yughahtf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2djitwnvt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axxkpszf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xgftxytv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzffzakr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoayatqc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ydwbhpec.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2trjzulfz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqwosmkj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zdkkrobe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pdkuavbj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cydgtcyz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bjmrpoip.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zuzexeql.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2btdtgaph.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rugylazz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2njgzwmga.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2stvdzpjw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lnnjjdfi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dywsmtkw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oiojbutm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vkbmlukf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yoepnxib.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tsguolmb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zktyekmk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tgekcxlf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2elorjwee.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bbbkhtfz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mwoioupk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ywmrkeuv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jyhxslej.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vvneyzny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ethldcfq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ltayhrjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfufrwpx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iggjsqji.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vnvixyfj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ybsnyedx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nlzvnxmb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vkwjqqqr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lqvdsbud.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rmzgpxhm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yjpcgdkm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aqlnsdlh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mcfbtqdo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2brfjgyzn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yqddrxma.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dohnyoru.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dvglhcdn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uwicblys.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mepvxjff.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fseymuuy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2potfmkmq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ooizrpxa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2cjctidku.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ztcwanlt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cxxbqroe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2sxllfwym.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2resrudai.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gepeixwo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wzuvdzuy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mujtrgaj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sarxgfzg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bmtbjulg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kvvmqmef.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cfjpzpxs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uclaugdr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dcbpkesb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lmhpbfcv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2meluqqdf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mtxnpmmm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bcqrtofk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tblnisvd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ranidkpb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xgrksjxy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psqbplhj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jqowomuo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2clgljzix.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2javvvbdy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2oitdgjts.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xypeydcb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jwhxbmol.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sskoxoji.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hdizspfu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bpikexvb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wpkluend.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qdanarmh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lwidqpkl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oepvvixh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ucfppxku.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kumygxky.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hubchytw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wyjksdet.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xgbfewuz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qccyjpvg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2shrnejqe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eejjnxkg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sxjxlmfv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bejwpvhy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ehrrlsii.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ufxsqasr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qsroclfm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2eneptrzd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xghzafdv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsjqpcno.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dtdblgli.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qilsyuiw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bgaleban.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ycgvqfrl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2seayqegy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2klbuwxdy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wdhcgnif.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hbyghvyy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2szsrerbx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tvaqcvgf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xsgybygo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xpaplbax.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxfoslqr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuxxrfuv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ruftplku.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nxqnxfji.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lyibrgjy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bdhbxpsr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2smwoxdtt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yloweyru.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sjzzxgdf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unbuchkk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2mgbefesx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ojmsectz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2eptsiuex.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wowfdyfz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ogeheqdv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xuyecegb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sprojeia.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ketwmgqs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmvliooz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bfgtgohs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hafzbqgd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2loiaehsl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gmopsvgx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tzdniymo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kiguxeml.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fsgdeixl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxjggmr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zjdsxbkd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrzjizhk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wuvtmnqe.html


<!-- 参考信息 -->