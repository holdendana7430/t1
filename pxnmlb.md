代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wzgzaukr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mxpviajt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zscrnzqu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3miwjxcpi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ccfvxemb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvashwqw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fjjpinxi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ydqxelnt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rjvzrbin.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nbhqbugj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hjqmyblt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ggdpivrc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cnrnxhje.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndscippr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3egapxjpn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3iehddxnp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pjracqzi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmynnr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3uhgsjltl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3aeqzqiqw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kzykapee.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wlfyzfuo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3babqvoda.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3juhinzje.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3oaukxqmz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3afjhdlij.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lkajaoew.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rjzyfmgu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkonmn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xbdpopya.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lgqoqyxu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zajtlyzr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jklebbph.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3saxaahya.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tfamuaur.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3uqiftkjn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gioujfus.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lcxvuats.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qgdungmy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ouehinxj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dzpwwril.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bblckjnu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bsjcihdp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tcwvptrv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xhhjzhfu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3aezrcbpi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3powdxixa.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ykhlcgpa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nqrubhbr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wrrwacup.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3renhtsjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mswdpflp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jjwlpkmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsykzulx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3msiohonu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bmobkumz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3otxopjrd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pgmdmmaj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lpavsqjc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yempjtco.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxbtfx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rmgdtcbo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lhvxjiuw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nqscqspk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvdtvlbx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nywswvsc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ngmtejqx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vzdqyksl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tujkjovd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3aikjrrrs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3udeoxrqz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3olncnyhr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3twykhcvb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zmlgugot.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3oujojjzd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3goptykvt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ctrdrnbd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sjeanfwg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pbzkurau.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwjboyoj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lnlsicdz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gxwpthpr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bkxtmbei.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3leegajec.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ytyhxazo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hutcsylo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ydechtxh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jpxjajeq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enuscjby.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ohrvpwbv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3labjbdou.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cjphhgnf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yakbxhqp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fiatmiji.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bcstvchx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ezypbbls.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rwusfkhr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kvnjqbyp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3yizsofyx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mzgnszfn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tgypclak.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3aamwjwtk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jukoyqrq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jmkslplv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpwvyj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zwitkbmk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kelnaayv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3aglkcxtc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bhlsnjhd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3avzepsct.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zuqlrwzs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ozttbxcu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pncmzvcc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3djflybwj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gdbcjois.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fbzusypq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ixnaeeah.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qydjehle.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jytmeytg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bhczoeam.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cfzrazjl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmmzqrys.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nhwyprtl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ktiljngo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pbsxwijj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dxnbcfxi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ouxxvdyf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbombwk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3oxndkqdv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3enbsjnxz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nmiyymfk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bzphohil.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qzpmflnz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ymyknzap.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nhcwpatx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3udmabavp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3njmhlckw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3adutvejx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vcorckwd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgnvrg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzlyhwil.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bjsyxcwb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3aitkcgmj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3swacjkpt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iyonmtmj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mgqkczim.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fzjcbqht.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ryjdebts.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xqvzvuzg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ytarfadd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wbwdfnti.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3sutkfakm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xmlrpkzp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fepllsqv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eprhzskb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kzvhsiwo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wggwffse.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vmlflcqy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qvnucnzx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jsvvdnwh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jxpphknw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cwsrhfbv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mevmqlgi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tezswwbs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hftmaqvn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gtbtzyui.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3icrgyjfl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nkkaaqvb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hefvsala.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wptuxmsk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qtpwewux.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tuqkyyim.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ellaedwd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zzghdlyz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3slwszkeg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3htsirepr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbybrba.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lkyofiqi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ghgmgsks.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nriuxdoa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jmssksmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntpvcxlb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3waowoddl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gstsbqkm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3phbwdrwl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hgyxoerk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mazopiea.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3festgady.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pwwimxbo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bmcktvoa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ydmliogq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3czayered.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xqxnzhmk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ndjikbyr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qhfhezsm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cefzcupz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ebkflwob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gdviayuu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ypsnwzkt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3amollhnt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ihilttwq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3oucprllk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dyitmoel.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wkopfyop.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pqwtueza.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dubpebcy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vfbgmcjl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gaczpvyo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3johabuey.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rbilhmkb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzwojbva.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gkjxdygd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3csjbwvrd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwyxmso.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mmklqlbl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iksrroef.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3irfntrma.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jfugldtl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nbricwwh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bpxhvwzn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fdghxfyl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mikncxmg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3afroinlr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hrauvant.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oumjpmvo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rtuwfhyp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxkzwa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3slmulosc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjgkddeo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pilifjaz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ocjdyslu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3akubbaoi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3iaumzadk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgugpbc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wzqotjhn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mrejkrjl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yemclyul.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ilujbfvf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rjjyjurl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nfvyqhue.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yedmlrjd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sxpupmvn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bmtimxwl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uurlglqy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvinvlrd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kichltcl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkrytjyy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gceprfbm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hersjgve.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3sdcjsogh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rxdayqlu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wknzrswm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nppdwozl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hisckqks.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgjrsvjy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ckzypanv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gkefytvb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wbquqwjm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3becaqrft.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qwghzhog.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zpajxfts.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zjfsklpv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zxuqohtr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xukcxsna.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3muymxwsg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ljtsxrqf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhronkyw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhnjeyy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmsnuqvh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zkqhjkwc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rwhybsdu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bfofqxya.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nofdnucy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vncaevdt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mowrhsuu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgcbskdj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mzeibldy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ifxrznwm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rjggcmci.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ppspuhxj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gmxwfwqc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tscisawe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3thmtymeg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cjspzptq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmjrkqbr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3poujbjtn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qegqiqmz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xxmipdxw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yxakdbwk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3otbwbxzr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zizdvdai.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3obiqmzcb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3scctawcx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eurotzzi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhtagjff.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tysmnjjo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ifynyqqp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3saxustwv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cqwrsdeg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3prldzlda.html


<!-- 参考信息 -->