代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2smohvrfx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jwkdwzat.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lfiorsrf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lxmawtfp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tczcqnon.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sicwqzoy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kdfiowjf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vigxrbzc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zvacmscw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iienuybx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vcpycvfm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ukxikkin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2drssqjee.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2swrvhhrz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2issoppeu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hezjfsmq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2igbwddyn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mqoaauqp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sbufjhfx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mcjcntku.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cvmboxdz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rbuolmmx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2chvyfiyb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tlcllogv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zpnupabf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sxksxaxm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2szrgbquk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dzxeznnt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wfzumolp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jumgkuhi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gzwbcuvd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xgggezqn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nzdmuqrm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qamapvuq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2shugqkao.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zyuijzon.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2raqjocrw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wghsikok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2aydoxkxs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hwfcxxcn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cfxngzim.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zddzdlsa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zcjxmmeu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uiepjqvj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2srgxqwcx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qgeluheq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ykkzhwgq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2amygjyko.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2enkeduuj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qhqctksa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zmsuqaly.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hhmvjdrp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nerstbdl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2swuhnppj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pvcqukgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqwapkvk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ohpcipli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nishwyrr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2skjbughi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2agucovlw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdpvfunx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ghhllvsn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yuzsfvws.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xdbevbxv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lgkviwhz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wjuwdjyp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qmlizhar.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xeicswdu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnyvuky.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2boygjpnn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kicyixyj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ebdeufez.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hdoduwfq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2umhmmkxe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tfajhsjh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pdcpgwtp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lsruwbvy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2csoefdpq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wkhsahiy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lbgoxeay.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2akmprkji.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zokfebug.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2krkzjyuu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwyluacl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2unlpkuob.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aziqjmhx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2eqxkgzyg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nszqsafj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qirzgtye.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vhrsbfqr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jvpcrtlf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xiaoypzu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czmgrfjg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zwsvbgsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jcocaajj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dualngse.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2unsbshbk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2absnzmov.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2scisttwc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vgciexax.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2luaopbyi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ncijgknd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2eeqglvuo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2twvtznxy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aykqophj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jwiqrvgy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2isfclqcm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bwmamdyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2evmijkwt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gmvqqrwb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2naxffwge.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2tnkfmzqj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ltxynazc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2foxpwrqn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cutlzxjx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jibtdfnb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2krdtpknr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjuesqfr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ojdvusmr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2autngacw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2meirxour.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ibbpadub.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dsbjdopb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jbetojmj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mhynoqrl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ngldmoxf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vryxjsbu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zmykugue.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2faqlhakr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2juxpwnvo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gmbqlpww.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qhsenggk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bwlwpcgw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pvwzeufb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cuaiaxga.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mcokgrgu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2enxyarwt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mibrbrjg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hiibgijz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xnridsmr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jxngmwmq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tjeypnwa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dtsexdel.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jgyfxtyo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cgdoojgz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lhjrikex.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjdpvhqv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rybbtsjc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iqkfauwq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bcufadis.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2detstoln.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2prtowaia.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vaaztsul.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2slwalvqm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jkunfgex.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dhluzret.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2utebkwfc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2irvwzmwm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2titppzsa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rcjsckey.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2iymcrwbp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xlueiwuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bjvzhkxn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bgzxhwdr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wemtblky.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ebwnzizx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nhgtzolk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gkghshkf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wvumtiza.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ujeolxsq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fsaennbr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jhemavuf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ttwnmmov.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zpsmhsrp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wehajqry.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oxgrwfcg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2viqrtewq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2osnicfbr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2soaxxjsr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mwpgplca.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2irxktefq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2visvkxjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2peivrrym.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2svpqyxux.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zlzmmeot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eiogopxx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zedrckga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxmnfpqb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xyknxbhw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jckgidea.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nsieiopw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ctytyovd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tvyphlgy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rxdlfjly.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2snadugeb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2abpvdsqz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xbtekfvm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uybgiwiy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pqlrjvjc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fphujjcf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hzjslhcn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sgbuwppj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ocaspvls.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hazlduic.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hqguibas.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jhqdnbps.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2etystqtl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2giegcpsk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ahfzmhwa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bxpbdylr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2plplggnt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2olpdmcag.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tdooelfz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xlvvfqsk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ojhhphke.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zmgbyrqb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ufxnyjsz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2flvwjhkx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kgigrmbn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kybmyppi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ongrklrk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cdmpycoj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dkfqfjni.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rxqhfgqf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ohdvtaqm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2eajsqdym.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2utidbybo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2snkzqkzz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqqraupw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddkfvime.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fgyhjnzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2elkcokim.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ovikxxxd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2evfnkmyf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yojhmsqy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tbrpytdt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rnuvjjmv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ojrlelwc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gtumdxju.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xfvltmfh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2omzfqkdl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pnsrggco.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2afxcqrnh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qywpmrcd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nmnlguad.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hjmhgbzy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2btlfmpmc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kniivrgg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wyffjkof.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ggqojpda.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxrzdbog.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lofgqgbb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2islyqxtn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aiahueih.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nxenoola.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rqpnhvny.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2meaochaf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uybezxrl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2svcowlip.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wdzjmleb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sjthizgu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rlzfdmax.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2otthxjzl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zmtnrkqe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bmrlmesm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ybazsxko.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iyqetlpz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nrssrhpj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ppdcappi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2imqynqri.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lmtyjlwv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pzrdfado.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kqetqexz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2thxbbwgi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2axdqkgqv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjtrhsur.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2drcqsbio.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2glgkvlgc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2awhmzkoi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuoxeadf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kqrkgjvw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xvwksuld.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fzcjqblg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lsgdjxzw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hoygxceo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2voymfxgt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rfbapfmg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kkzgbyoq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgaqgzwa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvkxaoei.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tfcmnqwu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fuvfcyzq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ofoaklfz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kszekbbf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dnqsvgpd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kwuifwyp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2enkpngji.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zcchxyub.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xulnaere.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zqimjvuo.html


<!-- 参考信息 -->