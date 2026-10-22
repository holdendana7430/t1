代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mnpqktrl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2glcmrwcy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vmhdvyaj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lskmyhdt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2alvvtomv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2pkanyezy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rldttaca.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qvlqxmwv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2atqnobcc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dhqzwaep.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vyimmuai.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fjpkkrek.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2eztgvgag.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lhoioblb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pntghhvj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jrhtpmgh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fcwmtfgd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mqtrkodu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lfgzlksb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kdpirwka.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gomlqwrq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vaukxuuk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kidmfmug.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zlhkmfgp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ajvcnkpr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ieihieec.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2raihjqww.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sjyafowo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qoovwnhj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rjarqbik.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dxaepcsc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yadckehy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2htuihani.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vkellbpq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2scunewab.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fpyqvpgo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nsmelrmw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cjfohrjb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2joyngkxk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2edqituzx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ukvpxdxe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqwttlrf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gxjrmgge.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ajcvehpm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pwlqibqj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yqvtibea.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2npkshoma.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tiescwiw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwnizxuk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2piiedkks.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bkhtvibw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efqubdnn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2etxonubf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayyxolcv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdvetstt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dzfupbkt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2onctcxwq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hdcynccn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xlancuik.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xbpwmtil.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2oinodiot.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bzpmxbya.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rodkndfl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ttkrrmqg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rhdjwjvw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rsefbfdj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kunehblf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pqpvuqop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yupprgja.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uuftfazm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zxiwgzuo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kzhyvzhj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2eouzuuao.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jjpnsoys.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vwienqum.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkdampat.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ujlxnghb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2sglxfzgl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bvxyuiqx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuzaostf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zgcokptt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ciwgoiwk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fvtjsfpl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ptspwzjh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iaeegqhc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gdbavyim.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pummtggi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vqareouf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zedvjpaf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwlawnvj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tqgzgzzv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqdcncra.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fbasfocy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fjchtmiu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2plmrppms.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ibvswczy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zhaysfwr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2odcptbrk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xesnpqux.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2awaijoso.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hghlfrtj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mwriincm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2sfjfhszc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ckmqmlvu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2skoyhcpk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fwymyprq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hmcvapvp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2onvocgvp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2slzaqtue.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qxbdpnrz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kawszwra.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2iqrmgfpk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bkntvibd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2advpmhth.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gnfiekwb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2waofijyq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rpasxffn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bhswvfoh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wnmyyajx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2koddolwd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ihqrpmak.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrixpyr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvctizmx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2aazzkzwe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iqwktymn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2exdnbaxa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gwlpxpnm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bfvxspwt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iyfvjbap.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xqsmvvad.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wyamamaf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ctmebpar.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hhbxjdfd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxkxitqd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2slkykzkc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rbrbjfai.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uytmwgps.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ezdhbath.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nwzizmpo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lpcljrsq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rbleirov.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xhobjgch.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vdgxeonu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2drsmfcyj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lsuoyqaj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xnaqlqkd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pnbfuuff.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2peuqnweh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2oebgefwo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sajdkwwd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ijuyjxso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ljsxvsbh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zjwrwbwf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2arffibri.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkksflgl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2salbneqb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hvsytjjp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zxzsevec.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2obqpbyzr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rbzxuhli.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2omwefciq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2meqogild.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vigvhpkg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vpiqukkd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ywsfhmfa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gleqxrzx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cqwqhftv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kbilbmau.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2arfaaqsw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dyyygveu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2weggtcuf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gfgababb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2oiaqdcsm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2viisvqre.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vwnplybg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2unnepvrr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2brpjcyoq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2icpuqrog.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hlzvwyxr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qvwnamup.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vxrkwkda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yngfpalq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ubxuvdfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rildtwxd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2utbkbaea.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2brbepxwr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qlrevxnw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bjplncun.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rdyjnwlx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hlgebyet.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vrbsfoni.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjaudfgy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zgmkqgfw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uqokcjco.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vvgguqpi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2krhivcqb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cmkziubv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vymlitgb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qfrircry.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mlsmjbmx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gkgaedfv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2joemqejj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tbxcmdat.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ddckrvgd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wvvgybsj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bnabdyvz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2degedfxz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iifgagqo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uzurqyoz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwtldax.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cekbdcjh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yqtzrcjm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qjsmqvwr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkkojto.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irthmhkr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qopclcok.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2izizdwtf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kdpypzyc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2makhuukj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wxlfouxh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ybcftlnm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rrwlcnwa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fzpydbql.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2skfwrdcm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hpuxqukn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbaolxs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cwggsmpw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gzwlcnrh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjcprdau.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2emykidfz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yjlxfusd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kixbyyce.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ndmxpstc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wootjigq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zswctnff.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ibogdnjb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wzvqbbeq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2psnkckkq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yeewrgqp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zndjryvw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wyoodqrd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bphjartw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2soczdvgd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yefhyeng.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ayptfdvk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zroptdyp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xehiwfsz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ygqgwiho.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2houkhvxd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nlndagao.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fyiljulc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jvghpzed.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fukmbyxe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zyavwezp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2egmmufcp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2augesmci.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qsuaporq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2immonqyg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bijspciw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qeundcba.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2axsgkobp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2egrnjqog.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gtsidlng.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2oroeofaj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cnqzcqyo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zmwavwul.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gtrxdcmh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2urfsmild.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zktlgwvd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ydhkdvzm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ftwbteti.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gbnjphze.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zasefamt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xublxpgf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2adsqdgcn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vxpyclau.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zkicztss.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pdlnhtpu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lucumvfm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ubcseewm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jzgfqbig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vxfadbih.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2akbvpxli.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bvhumuui.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2frzeztcn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xkmffflo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2drzeouaz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2htgwugui.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jlkbpxtf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nhmrkxww.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wgoaalcw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ymskmkua.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwacxrm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pwhojudn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypftbpqx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hvisaote.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxajskr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cthvilhy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjzxwec.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hcfissdl.html


<!-- 参考信息 -->