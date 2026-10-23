代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mxbywrfg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gpgcisaj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ofnvvxil.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ejraniua.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dwbtkmni.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gzaydyna.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nolqpkix.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ejbiaubd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3stlhpljw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcmatvty.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3djgwiuox.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3edzqynlh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xigmehhd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qwflwtec.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3piipymuo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wingubzg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pycyjnzm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmvwvohx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3legayfzn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uqkcewop.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ivdwnpjx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cylwpcfq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jmjqnpsf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wmlalziz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uxvnwxsd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcusmfkl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3crxisfxf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ltmtrfgf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fotqdigi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3dbnjpyos.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3etwyviwj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ujvkfjce.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fevwpolg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sftgqavv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3emnviweb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3heowqxzz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3owfllceq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nuqexzpa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwvinvvx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3oticwisv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nmslpqzp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lnsaljux.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3duixderm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zooqwsty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kxbhdaea.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lynxxvyo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lftzbbkf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vkptlnmf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3psqyljil.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3yfxeatky.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ngwcxgbf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xucgdxar.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rfszwyoq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ynobtvto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bqtlaxos.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jkiqysch.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3suubqpca.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3juvvddnb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3olnckosy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rlvrtuff.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3amqbeufj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hyyqznaj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3eaioqpvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwmezksk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3inwqmhng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bokcgmvc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3susqoket.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3dzfhapvj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxamamcp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mtoqgaeg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3japvkazv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bbovcqne.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wfaiprhk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3phxbzjvc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xilsbylk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3foryiktm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3iggtdnek.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oehqesrs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vgrufgxv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bynastng.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3nnawjtkk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kywvutua.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bnkxirik.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3areadpfa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gxgltvcb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3okawfvlq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bpiuqilx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ssgmiyki.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rpkituda.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mifwbpub.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cbvmwcsg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qlbsjheh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yjhikojb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgkjtv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3porkihpz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3myyafghz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3osgvzccq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oielbqhn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hdzkfcdc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cvgtzagq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jdjqivqd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yetezqaw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3akhnpnwm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3thcegnip.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yqvuxaxu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3beseouni.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3glknytkv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hhuxpwby.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3agylmzwa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fejzsvko.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ytcongmp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ywwfwxbe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3didfwmgs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dzboaioz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3smfmwovl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cissqfjd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bmejxeje.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zeaabbdu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nsajkugx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3szbniqoe.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ymvomngp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xqbsnffe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xkmgguji.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pivuukgd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gyxayfoq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pexaqohe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tzzovkal.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xjcupgpw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3idllozwy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xhzierxe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bqehrwmr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhpsdnhx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bwqelavt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3sokdyzga.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owtyrvom.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xcxwmebc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3emxflfee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mfioconk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dcyhcmil.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aannnwre.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xtlrgyup.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dwrtomai.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jbjcecrj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mrqituzw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nopbozqm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3htwtnbxt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vmbkadfh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fqlsjrxf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lbubvyuu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tbokzjfc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cpavbcvd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ufmwqqxm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmynjziy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cykouwpm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zpvczest.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dxjtrwqx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lixciobc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oteeqzpe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mbiqsmku.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ypflfxdh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vgeelpzt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3waaxbpuf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ibuwciwh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wljepvkk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gyusuqup.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ksygjwlp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpcmwbps.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tqglptwv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zvfkxjwn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajbrvuil.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jyniqdju.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3eggbjefc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aezraxph.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3teryotcm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3khkahtna.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ivxxhahz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfqbikvd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hjlchsuz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zpyuxycg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kjkedpss.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfyslya.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ydypuwty.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ikvjidqa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fbdzcykr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tswfltog.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3naiaychr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3olmmmxix.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oejhrklj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rgsmopve.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3eyqfkait.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vkxvpnuy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3scifxefz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sfolcylp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovhsfbah.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3spsiecti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwxclkxi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lnsqnnfz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wsuzfvcm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3aouantkr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pieewbtv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kvatgnbm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3muyzjnnq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3htgfxkhg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ydmozmrg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qlurawjo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yluusfnf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xhwedpjj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdbavda.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3myifrvny.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dhfgupqj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3iqmwjmcj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxayxnd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3anjvuknn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dveimjcy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bloaizjf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ppogujpb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xucdrgvf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxfwlcf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nadgrpbb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fksquyck.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lavqinzb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjwxefp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxipqtuy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mlwlaewt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3sdqunspw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iwelvaap.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yhhjprnu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uexmfvey.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3narfqqbx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwmxvoyo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3epjhrntj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ivgrlzrk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mtxhkjkb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nimwmpli.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hryayhag.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zfqaniyg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tzpgcrwz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uhbfonwi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eeedtllx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3neeeyayj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hzklihft.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jpkxotyo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3brjxcpwq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ottejrrh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3illgrkda.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3banbtjez.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gfukynue.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ekjrsdlb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vkjoqyyt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dlvlbysy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qlvdfgmf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gehcoxha.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3edfxxdwr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zuqrjhqs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ocuuvxfs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3afyfmwqs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xynrunrj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3syzibheb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qirgjufo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ojfbnted.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bohanprn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yigqqxsy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hkdihosk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3lycpwqwr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fwvffdfa.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zwssgiil.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cferfxfy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yxyttmrx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xpvwobzr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gbbxelvm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kzqevpes.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ribdhmls.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3boxtngpu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qluzvhnk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uzbueicb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kphncjwr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efpryzus.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kvnzufoo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3huxpkaxr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jaqbxicm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qdikdavf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yseilpav.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tlnuapok.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3raacxpeg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vmdpzusc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mvfvodrh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tkbetwqf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msvvnqci.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dnydlocy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mlxqikcv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rowjnafw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yodklczg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eexrovul.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grxkygup.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cpjqbxbx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3voeomdqr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3igaohbrj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pylnxbxr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yadbeqyl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyctxnok.html


<!-- 参考信息 -->