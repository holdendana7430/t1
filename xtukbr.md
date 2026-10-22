代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fnhugpfy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mplprmcf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ckxzuszh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2offtuthc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2itbaypkg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qruajlsn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2exzvqhnl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uuzzmcxd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kuelbccn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dasegeng.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fnlqxwno.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2uueekwml.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fdijhfoe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oiebahsq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yikdubnl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mtsagzst.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zzsmdgrv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tfgmlgjs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2giwhhyqt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2plmmiiaa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gcegsvgu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2oiorckgm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pgbmvjmi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iqhkvhtm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nepyrrlj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vczydexf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uqxeuazr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tiwjmcgt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ydvnxtrj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jqjatwcs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2igdfpumx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bnepyusv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uvxhgduq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vfguvctu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zreqdkop.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fshvbkbv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rvwxqtdp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dhkpjrck.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jdrtnkbe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pauqwvco.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wwcmagqq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2szcaozop.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2swzcfqsg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ipfptzob.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2izuzqtts.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bowrlbot.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cidircpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krcdbjiz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dczbsahv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsiseosc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hhafqqpo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rtbiizgj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nlpnvdxm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kcotvnse.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wyrzamxq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2saibhqkm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xlcvwfoa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wnprnxkk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hqppjpcj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ahdewatm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2myrvdvhi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ehfmtpsb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ylfqxbyg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yjcwdykk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bciyatka.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pggkfelr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ddoogxxe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cwdymrwg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2aeezxvri.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2cpsscnqw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bmylausg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qxweqjke.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2sbwvogrm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2eirsabmb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iagfhlqv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gxsnamja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2noctkctf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2updpzakx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pnlakazr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fjbkvsej.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zitmqwxd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hbpteooh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ytsvgltf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lsxtgfxb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nppamitk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usanzdgu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jfvqoemf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2chfgpmxm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpeulho.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tnggyltz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hvdyslkc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2crrhtilh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ldqlsmem.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2syotoirq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vnskksui.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dbeneecb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ppfvopsq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fbtsbfdd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lvojdmud.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2oazkkula.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rubmcrim.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ulkksejl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ionwytrv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pylvyaev.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dzxjtqtm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gsnazwmz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rhdpilto.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lnjyamtw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mkuwflpn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2axgezrim.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2axstpbyl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qyoayjhm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pnuseqid.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kdhhrtvh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kxybqfds.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kstzzxzx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lejusrnt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drnshanl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sksuvqim.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yrzonmvj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2arguufye.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nnunrdkf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ypajlujl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eotzeinf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jqsxuweu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pllmfwvy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2okpjilih.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ioosirnl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gilzigcg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rmqyocmm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2johlweyy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sclgnosi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bqwqbojy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zzahicvj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pgxjmvzg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lrqzscrt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zjxmbkfm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2doqyioam.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pigoovzh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2aaxepokn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2puvsraqg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vseqhcnq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vwvxfaia.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jymxitdx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2likhadiw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ralxervw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pkdaluhc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qofnpnxo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fgouykep.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdpccnn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2flcrrkvj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2achytihi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jnzzkczc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuifpahs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ayogrcxu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xciaptum.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fgreylfq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2svkvfnbd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nbjbtoum.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qqbwhyki.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kzdialzv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aqofzwys.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ydnvnexr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pyvblqhs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fifixdos.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qvlfxdld.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pfiqsovl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gdaazwji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fgauszeg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zhzoaaun.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mqvdxwpy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tjdvesjh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lklpaslq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2krbqvesc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wvllsork.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2smxyllni.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vlerbhwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzulowpb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qybakwas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehfwlgon.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pcqhihfm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kspzvmgn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nsqvahof.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ucuemaur.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lzvyrtvk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dmruckmu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cvbolryv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xloknbxr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gtnwztxz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tlfakvzk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jfxgyuln.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rlzfxfhd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ezvqqexq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebxcxszq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ncaympuh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ijanyouz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckmlvyxs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2blhlkksl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2adifajvv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rgqprggt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2sktdjlss.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lheqkcdt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2cnslsegs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xbwuiprc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2juezsiam.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxllnd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ydebrxyi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kafjzqru.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2iojmxwki.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lerhddxq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2illjhenm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qeuavknj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2iixfoeha.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2loekaune.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jfhvpcpd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mqiapiqo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2obfgfqfi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rpdlbdhh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qonvbtaj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gwzaptlk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hzpupmri.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2edanubov.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2sorvgtvp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2clvuaquo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzxzstzy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bgmxdqcc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kfibgdjp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ofhezrof.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hpnmaier.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gekrmekw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2eltwznio.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfereuc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ngjtxxlr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lwzqojdm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zvnliorq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2umrqutlo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2eieciocy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2crwbfgwh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hxxtggfm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cmxydhnt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sguuqljb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2smaquiwp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2doeflxhh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ncakvhfd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xcjbdrjr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aefifkaa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tnpcdbgo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zpjlyphr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xfmzagqh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vsrrseoy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2stqgokvc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pfdmyuhj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hrlzkugr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2shpvsibb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qpnynjwm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dbrhaugg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tsheawbe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2notdpmen.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2frtfazbt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jdotkmsn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwslpuzh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xzldylqj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2foqxfxyg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2yiwquuon.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rhbnjubq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wkxdqvqw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2oqzaelks.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2phpokqvx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ssmukoio.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqhsbtvh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yzwcslwy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wcpxtpav.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pqyznoya.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2acickcaf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lnelmsov.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xlkhlsbv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2sxpcjtii.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2epscjdbz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2icuimwww.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2npzlmvhz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjthympj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2llyduyge.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yvmeprds.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvfiqumb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2aapclxmd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wduvbjhi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zeqxfvcj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qjqsmjtl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nzfzfwkr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xjzledxj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqqgvdw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2elczhjhg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2loymqzlw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wnlbmaem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pkomtrjl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2slffyngu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dqjnkqnp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tblhmymb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ylfihnrm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2sresaymh.html


<!-- 参考信息 -->