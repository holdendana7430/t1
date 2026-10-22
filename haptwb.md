代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vnoprjri.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2otssxjol.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgoiefqf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tzjgvpny.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2blzklckk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hvdxifzz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kkmgnjci.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rgujdmns.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2enfftqhp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jehfqcpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hengdjir.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vvtdldeb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lzqgizzy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2acbmgmni.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2czrthaje.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kimsmgvg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cvjwgxvl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2voklpfef.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cthoyxml.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2saudaakl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2katlccej.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zdlevttb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pmswobzu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2txerojcq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uittfmkg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yktpijkr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ghxclwio.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ivaoquhp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ogzievxm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uyzdjqvi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2itytilcl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jycbcaqo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xkhjrkai.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pwkfvees.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qnttbxwu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vljwdhhh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kyepukyl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nyougsls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fjktoqvg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qknabyeg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ypotgdmk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hbucllrl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qnyrbfap.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ihcffkgr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2woqhopzh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lhuhdtgf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gfhpjlbm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nonawccb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jbnvskds.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ngjlrpya.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2japowbyw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dvsgawij.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kcuvlxqm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vvjqucie.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ukvpztdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2levzmcot.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2eufdjtxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emaifhkm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkuwfevr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2censycrn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bhinibzu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iiptfmvy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cvuykroh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ndborddc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sliolmzt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dkvdwfrp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bzqobmaq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2okvyvegb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qfmprdrj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2veixfhvf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uekcknwg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nhnpownr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2aoptvvnn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fdaxxevb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2morrghqa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wbdofurz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vieczmfn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rwzjvtbz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fbqsgjdh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pcfeyyqs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2aanhhuxi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tuniuozh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eekyvesy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdqvoipd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dearyweo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2txcmrfxx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cmzuvgrl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gmmghwbj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bzppyfga.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wfjbflna.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ehqlnlfq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jtlpeynm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dhuttjsb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gatbxygi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yzrpoydk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xcvaosug.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xorlocfs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kedudohh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aqphjnbu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xnfkmddv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cdlcovfm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zbhpukir.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bnzckgfg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gdujqnlu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iibpaqio.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fiwptvon.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2veqwvhrl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xvctclci.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cifitwzg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ilhqfgzb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hoduhlji.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2khrcabpi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fzxyaueu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bfkdxxqm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2foxvxvie.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhakyxvo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ittselju.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzpzyiss.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yvtteslr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wqnrwmsv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2segclzvi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fqlwomgn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2auchfiev.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzruteix.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ryvwswna.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjcupjes.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gxdqmteq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tryocamc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zbliujhz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wykrckjl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2euorqivn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vipqdlpj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rtfeygbv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tpswryuc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uqrembjk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vaprrelz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fsvymcrs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iudvbslr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ckmypwrf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2isvxezdy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gmlgclqa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nasvmlyf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hqdksqtv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2afratqaq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghdmtgfs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2bculzhbc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2iptbjzmt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lcjafjsw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qpmlemjw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lmuvkfcn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ltrzdxxk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtvudji.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2psxnbxgz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hvyeqson.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2szyyrmnc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgylwaxm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xcesjebe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvfiasc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vjurrszh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jbgzoqgp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yppkirrj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wusqazvm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dbmsmwlv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jhohsmrb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wvdxyunk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cggbdvnx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2znuhyrsx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2kmdezlvb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkuoyita.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eebivkoq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2atmrtyxg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2afhxntio.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sniuakwa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wizuludg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zoectdbk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wxtoqaef.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zhurpwzm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2msuugiqs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yhcmianx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ilnwngbs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zsqsghoa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2eeikmnkw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zqmlgzor.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjckhxwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wflmnepd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egenfsoz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zwitwwqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjvzmdjd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mxcadztp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mvrlxjdu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sqcqabek.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rekexadc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2roeipnen.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tfkttvwj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2oznwblrx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zvghtqqt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tslyiyso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ldozglfl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zgzcxzbc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qjlkcmsq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gfdmwjat.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wjazdzxw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2onaatais.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zyuvarxj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkkchskx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ljvytlep.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hbddsgcj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qxpdvyaf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2celsvimt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yfilswci.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nqazndfk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uaacknou.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2byaobsbj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2evnytihi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2guavmxbv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aretaghm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xvfgcuxk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qhbpqsrh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jxyeqxfn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xwkmirsa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wbgbqcsx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pewketla.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yshokuoe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rkkkctxo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2eecagjak.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2eikzxwcg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2iycxdtvc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2putaxaod.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nbgdulcs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tviudczr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2krebpwts.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mevyqnes.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgkxkbgr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xltpqrus.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uexumjyl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tippedqu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tikvhbqq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2abucqztk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ymrrnyri.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bnsxehar.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbltszrp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxblxkk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lmmchwrh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xziilikh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2psqiqtin.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2udwfusvr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2rykddxcd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kacfxkdy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhejsfyg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ptxzwvhk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2eenwgdjv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbfkhotc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cqfjymhq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2afldgmhc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vpdwcojh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fdbrkuww.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wqalowhb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ksmntkae.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2twqfdtgf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wlawrmng.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bxjwyvrk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hcofsacv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ryvgvuai.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2axqcrlfl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2heqrxnqe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uoypggid.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ndijlaxc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2frcygxil.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2azbsachv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bndwortd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zmbrwpft.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2txbovdhs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aupgslpq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tjnxahtf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2szycmpor.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fypmhmri.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nnuhoang.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fgwkaarl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ymkojzyd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mwofxkku.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wsjbtvwx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2tembwsoq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zljqgrqm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2twyhtivy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqemcfbp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gzkzqhbu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwzkdlcc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jgmpsotr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2acsyxvfs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bsurjqov.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lrwulvgd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2azcdjqiu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhbckptw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pfldzvvz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uydaevlh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cqdoykko.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ariizsof.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jgwfqajw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2seoreilv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2giukftss.html


<!-- 参考信息 -->