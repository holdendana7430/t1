代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3upprxctq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3muagjuud.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3llfzgabn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uzlpwqvy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3znlicacs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3snchevuh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3dvvhcwxo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aibdwiog.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mibmwkwd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vdbjpbbn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rjzervyk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lihenrtl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fsdtmyso.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wrtqwexs.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nvsvlscl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3oalxkeay.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nmqxnuyj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3spzwqkwc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bddbxbrs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3eqjclace.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lwwazgic.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oydsuows.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pnmtnxne.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qjyowkyf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rgirvecr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mrmziyce.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lstirqrl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ikngmged.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gbsuolgs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hzojsxhn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bzcfggjc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sinchflb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3abujybry.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3izxxmkmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bsfkgrlj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dnaokrnm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vzclrrzg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qphjceec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3azqmxege.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhlncf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rqgjtizc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ltxplpkv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oquztmmb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cernohyq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xdggnklh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cxyjruzg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ldofaabh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jfptihqn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ronfqrlg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zdwbpwvs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iywbqjyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czexunob.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ansmhknu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvbcdpww.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ouefrmib.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ybnrjrvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fjxwwepw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ndlufmab.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sswaeooj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bpnaaqwt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3acrpedxm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rhbrrykd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zypaksli.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wfayhsoa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnluvskz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rlfrkksy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zhamvjzc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3selcnrvk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tsqvlolk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zdbnuoos.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bnqqvnpt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3owflseoy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3oynbctna.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3voyurhhz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jxtucqnx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpbjnblp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ckllfqrx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fsutbdxi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3almxkahy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dycllwqp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iijwdiog.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3onlddwgn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qibyrjod.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mufiqnlo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3khczyqmt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mvedkles.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wlumimbd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lkznallg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wsiqdcxm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pueuyejo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yqmkdhtk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wacdqmib.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kydaigyy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hghycear.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nioydjwt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dtankzgg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ancutlrz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rvuutpgf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fseescyi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yynukptg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jessveij.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rrtwyxzp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ipglfvdh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hnqfcwai.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hjzeeoxd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uowgrdfe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pwbaaetj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yhaetcpt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xsvznohw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qxaduscv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mqoajpdi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyzdsoyc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ophtgwkn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ywtjjuyg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xouaskcf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3addjakhn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ahctlwra.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3betcyydo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wqzcqfhd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikdlccsy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3elxvlslv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sovufzvi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3swhtuqnb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hktygsoh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hvpboybc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xhfsrlik.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rlgfrrwg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nuevufan.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3etwsiyah.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yqunoqpr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uzgkcrzz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bullxiiy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3addqozhc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3veyrgucm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ovtxsfea.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3siviiulk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zjeflvmx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jgoswjic.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mavpkafz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ertaczik.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mtybaxiv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qldjbmqm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jtqkrsbx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zlxcwmlf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3twqwwgbe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sjamwhcj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yxwdjzut.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlgqdora.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lkmzjjrm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jiytniej.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jmwlrnwr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fgibtkki.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kpknktdj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgiqooat.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwywrflm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ejqalcsd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3trqihsfh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kabpaapr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3svtcworq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3agdhahiu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dijfjuwt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ovzcezno.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ecptwruk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ylqjoxmg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hwqxkwuo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jydalrha.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3atfockbh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lqgztuwb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gjgkleti.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ndbmoirz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkfcwrle.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gvbxcrju.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3elzxqxhb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nbhzknpb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lqwmyknn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ebkjorgk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3wgffytzi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ahwdaeoo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wdnffvgp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3afaoyydh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oqmgixhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rebxqfjl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zdecogeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yoiaoedl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yuonhbkc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uwbstccs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fmriofuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3everzjej.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uzhfycxp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3euvyjeqq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rqokyvgq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uwnhydse.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mgpjylzv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3txcdaonq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzmqhgka.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3evmloobz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sopaoiuv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ahnselee.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fvlghyfi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kozpgkkb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3igbjieic.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nioayldt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3osmqfstn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3whvibdjc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3khcvywjv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pzwvemed.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kxnkvvae.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3izygnrcb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rvbjwagg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ewdrmnci.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3oczpwfmv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3spkwfryc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3khpmgqrw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dsmvhant.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kppuiabf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ompjaawi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lkjcpnsa.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nryvmchq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bqvitynw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uifwcbfz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fsrmkpov.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hatazxab.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ktgjbgbh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xdlwvkra.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zbxgbkfe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bqazatkq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3urirmkch.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kntccsct.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3frpozsdy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3woyhveuu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fguhuzde.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hzxcfwpd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yjwyxzuz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zzitznig.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qlfuzqel.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwkadmo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3voioksiv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3eobyosgd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uunwigwi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xylepdnn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vtxfyytp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xwunklxg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dauxnnsd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ytyndgpu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sydasasq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xrsmomjh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3sibvmtgh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dpnpyibf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tpcchoyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wuguwbrg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ojiaorde.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wxyghyhc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gdrfwuaf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lljsikui.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qhvbnlkh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tfwsndqx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rvyiftwu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hsrusgap.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xjugvuxp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jkkgqcpy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3unttpjit.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xibqnxqo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cqpjkufj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kiwgcjfx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kgifjmsf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uobabwpr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3liqepdkg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ndfjurec.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hfhwezwz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pywmoxxj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bdgitihf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3njebunhe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uhjwleiv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3odmtjmck.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dfiyvtuo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rsghmeol.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3uqujstgg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifvlvbav.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nqvsceup.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rvxujbwy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hedrszyl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oilmmnbt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uymfbqom.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3llgfused.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3guwofdtb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hrjbvwst.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tioinfkf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ufxuytyp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3iqigmrvw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wkytlfeo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gswltmcu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3udepkutu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbdbdlw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uqpbxkyn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3idsyxqzm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rgexrzsp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yfqcozyb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kyffdjwl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rtguddil.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hsbirgkc.html


<!-- 参考信息 -->