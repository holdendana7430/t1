代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nqzulksa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3acwojgkp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ionlxsko.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bqvqwpwn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kpjrllqr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tunrspgz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3czltriny.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3oljahdss.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rwlxvpje.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bfstmgbt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jdysaoik.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3djlqyaxt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3axeumokj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jhvfxfeu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3beizwgag.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3alfkhqmz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qmopxprb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nuoxulmv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jvtkpodu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3itricfhz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dnxwpivb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3adsuymzh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zmwmagup.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dxnunshg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gmlgyhhs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fuikkfzr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nhprxqwj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yyotgcaf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tfhrikbu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3twhhvrdc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iyfecino.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3awgklujg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3giyolvch.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3uieqlqeh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3drmqiogt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsoycwqt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3aynrmhnd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lmypxpbb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kaxbhpts.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gvtjluuo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zhktwsnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kvqjjast.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xnozmmsj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lwvdwjdc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3onfvpihs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xdqouknb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3isdhemen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zulnzbgg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yfmpxwag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eurvxjli.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3siliptnu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tazpfpfp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxzevqhh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pvtuzqxd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kyoarolv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ejzbfqjw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wxcbpgdl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xbfyovce.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3abjtshcn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uctppcmr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lutbazun.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pzoevppn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ncilydkj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3alghdkrv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gbmndocu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3akzihjom.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3whjcxggb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mubhdfjr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tucbzjhb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gyqlvirk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aysrdmbi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3guonjjjy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yjudtepu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3caoslkgv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3asohxlmu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbzwfanj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3reihrvfe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jaxyoike.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vbwzozxl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wnzhqefq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uvlehreb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3omcmdjmb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zoaxcshz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rgejwlzv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cpnxisyl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hwqvdsxw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nbczzmui.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lsrudvpo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3afxywsij.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mquvsdnk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tnswsfrj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mijdjmws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3blrwzbzw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wrwkbcgx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qzaigalg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vshcqxaz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yohaiqxr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lbnfnrtf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xqnkdwbb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lrrmzbyg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3snuazbos.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fdfpchon.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hmftsbzf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rfluhhne.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dpcuxofa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rqyqlylf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kyahsedi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zosrrojw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zuxpmkum.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qpbuppng.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tmbukvev.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wycragkb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hvbvksbi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3umwvimao.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pvndqpoa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwsvorgs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hrktwdvg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myefyouf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ydxhwxdc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xlkbmqlb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ojmmcsgj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vznthivw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rlxntgwr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvdvooud.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hfspxpoy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pbfvlrvi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kguzwcwc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sneicmhg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cmctjtac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dfmbtsam.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qxohuxwi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sbfmrocr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dmjnfxcu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3llixjtmm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3aiaglzis.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgkbswyz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3okbjryii.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ccvedqyp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvcxtzro.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eicqzwbc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fgcbpytc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vfnyvcyy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xmkbeloi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ctelhywj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nykovmie.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cmvsnctu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tvcfyqro.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3trnxgjby.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yeqbqcba.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzroqfoe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmpnanac.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nsroigdf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3numpbnlr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mqluwurn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ynwatssq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rzyplezm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yntbdztk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3flhqjfhl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mltunsmp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ghtammpb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3slgxbsil.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mqjdkqjf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yiubmoys.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kvtmzuzp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hcbrdjix.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3czerpojd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3svuqgjgn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tzplvkfb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3udjshems.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fqpxkaiu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zryaobhb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dyskpunu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fkqxqrhd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hasfcohl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3senvherb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3oafqjcrj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aaemjzbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moggdaiw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bwvuavuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrmfpvih.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pfvuttnh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tkswvevx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3erxfguqc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bwwhfnli.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3brhtrtwq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3krzusnic.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3txtrjies.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mlvdkuvb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3okiwftdb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zavkyqcr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oollugoa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcpjimxa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jscthpld.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iavvzont.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ikhsempj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dwcxtmsp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxokwgzo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xniqzlei.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldsllltn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qheooqcd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bmpwlmta.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xfkdssey.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hwtxrksz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrxioqt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lcawfagz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vlmemgqj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qexuvnil.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wheqgdee.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wfkeuele.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hftmzvjc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3abddekmd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vxpyyktq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3iyqmpday.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fldswedk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3krbcqsne.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uudklotl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3htgwjvml.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hswutyej.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3akhiquwz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gujqhmhc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3llkbftxw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxtglce.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ymjcjofm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ltdcyifu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vjbenreq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qcdlyeph.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gmmwgyng.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjchlvbh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pzvdqrbv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dqiqjunt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mrbxmgdp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3waeetwyu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3awakwkaz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbhddnq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qmgfsoue.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nyuuyqtx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xbqipjyc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3isywbqsg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3eehwhvaz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iqsbozpf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdffbogi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3buzucjdn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hvaoarto.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kszobhru.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tedkhdub.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3prpxklmh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lzyziacg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3oguiadal.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3izhelkot.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fketovcn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pzoyptmn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wsxemtdp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ikiiimjv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hivsette.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jxyetznm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vywjyxkr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fdfgmxva.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eqytlyuu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yllqtxcq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qdyhdenx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aoiyebbk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3clkbsvki.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgvgzmwa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3osmietvq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ymfvlgix.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wxhdfbfz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bjiwghxz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ikyffgbl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nnudnwqf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kayiuflj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gblesqve.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lmxhytlo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3drtvkwht.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ljxxtmic.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xmhyrowi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zwnqcqti.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yrfhjada.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mbjlkzyj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mrdlhwab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wpoajfjx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgddmicz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3judunwfc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qaroizio.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uutztvuq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ofbdguxx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zbsfavto.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3txgtnzih.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ciyfpnxq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afoadwff.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nrjkvsfr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3txalfckq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3uiaeriag.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3thbbgxti.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gfeahpxl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvvdvye.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3totozpaj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3osejshcm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zywmixdc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nweaippj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nqocogtz.html


<!-- 参考信息 -->