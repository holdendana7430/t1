代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2juijsvgw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zwuhneew.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fsorwjaq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uerpapvb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vxotuqlf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqziwlqp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vdirrwhp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yhfwpils.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2prmqerog.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2igvexpwh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vihdxxyc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jyipdnka.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dbcyrybv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2krryboik.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qvaawrks.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2csnsznif.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2eoerpddk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qzyqyfml.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ewpqsgsv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rjrhciaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2femlovkx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2eundscsw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2oidfkdzr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tevcobei.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2scnmbblo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2woedafcs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hoocdowx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pmchesfy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uqrqeddj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vkdjeemg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ckjtamdo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kuziirym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sceqaeyz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tecgecfq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2efclokqt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fwfascer.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bybtrrld.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xxvgszly.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlmgcmmy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2uufgljgf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zagspgik.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fzdfbeql.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mmalhjtm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jijyjwew.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2upfjynku.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2pmhevlgw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tpuoktdh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qtcmtdsc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2etbyumcu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bxqemdky.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qxwkqwov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttomnnks.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jjzavsdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohfqfmjc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gisijspc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dhaqzorz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2njojvwyj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2oknselzv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nihpobvn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dwfcofhb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ckbfrnxq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2faqprblh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2litlwznx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2awigottj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dcsnalqw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jvihmniz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vckyrasa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rreygkvl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fituidjd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ihchulpq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wvhqrevg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gbkrsixb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mdidbooe.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jbxpyprs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fknjcwdy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqtkrymr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vppuaylk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fgwwgxhq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2efcdevrb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gkpobqwq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uhvkesre.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dnpqwaic.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jnrevltq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bwngcgkk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qxdgzrbo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gugzycss.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2oihuoehp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uoastjlq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfjnkiv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fugkpifc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ifcjsxrr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcshkgms.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eacujgwr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lnebhqtl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vrsirifz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qdnahxkq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xsuxdbgo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ezktyxkg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qclfgrla.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kaqedyct.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kmbfpjka.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2igsdglpr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bcagxdlb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fnrlhrxo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wrcbghhq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2walruclw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hnaxadke.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mamysbru.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2exbzaafm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rbpitomf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nceeyclo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2agamhseh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vbnvfkqc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rtxabzhp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qbypryei.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2tkqvykcs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zmyewwgc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2oisohhpz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rlhsehab.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oruwcome.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zdfbuigx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2nzdhpmvz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2akxtyusb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2eppkrmdv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2suvhywjr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ncqkxcku.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zclwjdgn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqtzmigz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2znhxylng.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2edfdasuy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vbfsxgfe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2povshhju.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2thjhwbpw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lztuwufd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fuvxsiwt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xlcfohil.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vedznxlp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qstiljwr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlikwfdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zaztegsu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dpdnyyjk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dtqqgwby.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtacxzxb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oepaxrti.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zqrevjha.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yxsyrjud.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bchdwhsf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcpgiply.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wcnijoaz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vcnyvtay.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2llcaulbz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lugbujqe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ctpzgrkn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yewoffeb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hfqaizml.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ovwqwgbk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbcvvf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wvmcuope.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rwmfokui.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2phseimrf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lxfukmul.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jpqwqruh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cptuxzhd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nwvwsihx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jkaozops.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eyyhvxyr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ggqszsla.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2illlduub.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ltmlgdis.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nhuebnah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dcxssrjg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kcdyhovq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cprtbxrp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jggavgwy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2eevmjnbm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vpruxhtw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vkpoksrb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pctjlwle.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fyqgwlky.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2eydwzfsh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2paxrgfhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olkqnmlu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gesvaffh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dktwqxhk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zjpbuflo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ozaxjnck.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gibzsnes.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ojdherbs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eqypobcj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hrxwnkzu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xyodelma.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gpxzfthy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2benptszf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bprshcif.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gkxortit.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2coxtebum.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tznggfgx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pyerqgsn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zywcmfva.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2womucfwp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2slznpjlw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vnhapevu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uybwerzr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2amzurfbo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eptrcyqy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nohkqquj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uvgxkykv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wrgkdyjz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qbzpuiio.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqolxfl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2iccpmemb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bfqcsfla.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2szpdcqfp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rxnasgir.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ihctsgrg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wzsdpkwk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pydddzex.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sdtrgynr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bteliyuj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ywftlmns.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xkkuiyxb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vtxrpdbj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zyjeldsr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iudnvsxl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rgahqzwm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mrnrytra.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqgfck.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nktwagqt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbsufvgm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2twlcrznm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jhtgisia.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vgcpgnjr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ndtqnjdo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pkecayom.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zaohysjb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vgfjpapt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbkdgtvy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dxrkjavw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gaotylnm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kqwkxmcz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ncjhvula.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vexbmqir.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hortgsim.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rvtvsvfd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vnriplkz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dtopptyd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tttmcpei.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywiosxny.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2iuonlyub.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jbyfxeub.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xmqslmpg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zuuyvbac.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pqbdqrmz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mfqbapfj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjitvqgn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fxfhecma.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rqgdgqmd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tptyjvbs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qfvdczdg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2uzadxkrm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ufznchuj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vgivvvrl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ipzdxsbm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hibitpec.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rbtsxxoe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dczqmwmh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tvkkkuvf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ckywdlny.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jnqsugga.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2onconlzi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fiywzhnq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjvpiqrh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2swxkiqdp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2khykwajm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jvoeffry.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fbudhelu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uerdbdil.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qrwuzfrx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vwrwudgk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fewpzhmm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2minnrnsh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdukglbv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wyxmubew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zgjazyre.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yyizqegr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cnpquirn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pwlhkqkd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uvgvjqzu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qfbmposp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fhkagips.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ufvsjnlq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2suezgxgm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwmrmnc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fiyzwbrt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnlojhsf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cuxmqcgq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2whxbusvr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2giflpzho.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ukemcuko.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ajlsahlt.html


<!-- 参考信息 -->