代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vfjxldod.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jrnayhfx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2teesfrhi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dizqkxew.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rcxqrksk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cunwddgw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mtcdkjcb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qabodzzy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2syralyyo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nciahlss.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgalqhd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ddjyzpdb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gdogxeao.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kgfeeopc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fcuwwjsy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vjslpwqd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2enktyuxe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gahcgwvs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2niipxsvy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2acdefllp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lfaquvyp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ljqqbuvc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uvojkpjd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mrcaytlw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2joueamaz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lbnxcqku.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rjmnngpr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2imtibbbk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2noegfwdw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xbmugofp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ekvizpsk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytnmkjfm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2msrgmqbr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2snellwqc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cjchenqb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2grjxbcnd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nyjmdisy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2teggkrsg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdgmibki.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rygforcw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rnxlfgny.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2juyltett.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ucfmamog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbdpqrds.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uejmtzbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvbqroxu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nlitylvm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2seqgddux.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpbkttpw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ckdcdsgf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xtpffsna.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2imhruypt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qztdnwyo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2awvnsumm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mmmgaiwa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zkaaafmt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkdvbyhk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dqndelag.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rykhanru.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zjiejujw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lfviuzsr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ggkrqrsx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2robvnqkv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hsebtvcn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zppqduhw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iiqsxrak.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ewpacpig.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dufvnuaj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fkdivynn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrfkzmh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vxoqaoon.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2njdiudhp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yzlixacx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ijgehcch.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2yufhilhw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2liwmohmp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rfcqfhdt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2godlurth.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tqvzlnef.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2reszntnx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cskldjxm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ifwpkjdd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2uhccodls.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xzdolmne.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mtwyrfzg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lykkzcic.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zygsiset.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2okyjaeqa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jzvdffvr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2oneiqrsr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dkvxclds.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2poqcknaw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2evoiwoxl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fbelrytd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2npwghoxa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vcmrzrhd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ajezziwz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tilfsxnc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kanabpbm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ewtdkvvx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wycznwob.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vrfmddeb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jvpeocea.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2migilwcw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jeoidvpa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vivtbzjs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vsofzzbm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ehjaitre.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nkmebeqa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zqomzaga.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uainoini.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2flfvdlag.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qnovjcpm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjkqydc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2aubsddyd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pkstmgys.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nnerlghs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2eemwqish.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jzkztuoo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzvxzeb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wconwpyg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lisuqzfs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dsbuelid.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wucgsskm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cpeqirzw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ldcoxltl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tdjkmasn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fxkwhnlu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2aotumtlh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zcschopx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yxtmnoed.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dokntwgh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lldjzubn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2odeogngf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2huqpviox.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hbzvzams.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nvwoocre.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yovesixb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2racdidvx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwcfpcxm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2eisnayes.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ouxdhoso.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pzganbhh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmciyfj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hsrpanip.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2otuffllg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bmbfjfsx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2osbyrwbs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bphnglsq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgbwmhpf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gxqlspnr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lextkwlx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tnegqetl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hywrriha.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yspzfjki.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iruwgkzy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2igylgvue.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lsiiodcg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lckommej.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zwbwyfdk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bachtlop.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dtjemfsd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2buqlocgk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2iglsfspr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqiiktex.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjioxp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tvwulvqi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kvayykiu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anniblcn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2thamlbzz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2iojgiojt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tjybrlyb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jmcvgiie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzlcvamv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aqqaaucz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amlhjoqm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lcetcgyw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xzsmbrld.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqccdvyn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nlqefmvq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wtroytnr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wzkstrtp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fgbmrzqf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lxdlkgbe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dpyrjkrw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fcwasohk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uckxuhxx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tcbwwtte.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qqtktjks.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wxohhppl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wxbrymyj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdavyaw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2msxwdupl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hauacdbc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ldnznwap.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nljukdry.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lymqixif.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2otkgtrhi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zgnpttpz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uhyeunux.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2slfrnxig.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xmkpecgf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zflajkqj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2orxuddzi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vxeeqard.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2oypmkoxj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tazkyefa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gqlvogwc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2iphkxxzl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2czmbpugc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxtpuyqh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rjrjjlwd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hutxbjqo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2frqdgfvw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pjitwwta.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iamufpan.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2plbbbgun.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vzagjtan.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2trlhqubo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lclqxuhf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cqinflhn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2syslxdez.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wgcoenqn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2baorcfcp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pumigkaa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tcjieyxc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2iunwfeqa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ypgubvdb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xzobhgci.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2eveqfdhw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dvbxxrkd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vokpzhhv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2futsmboc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qxitvcrp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2eodfjjmb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oezaqaun.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wyddqwdk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2otltbjth.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bvwzdxtw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kiionijg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dbrkufet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2znsgjibo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wcucvxhh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dbrzkchz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bghyclgb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2woxylvbq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hamorqhz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2eimyxrvk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jxqazwdh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ggjrbfty.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2djiqegdv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yaxfblju.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rjkpsmyd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2migolmbd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2skvjymsk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pucuzuco.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbtbvyce.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hnfzcenx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2egrhqzfh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2njsojksk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ngovvcti.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bruiaikf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rkndkyke.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgaytdqa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rglhqwdi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vqbqukyh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkycgufd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zveikecx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jzczqcdx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcwgytuh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jldrfubi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ghqlzila.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzrczuxz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqdwzpyg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lypygrtc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wereygpq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqkpinwn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xcymwecd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tggukkdy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2loskrdsj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gpfgnbsx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2twmppmag.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oyrclygb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2snapwueb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvbedrz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bpinooip.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yupqygix.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uqunvmyf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fgderbfi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2upvzoamg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zgilnsxb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gjlabcoe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cldwhxyp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nofztzkl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2arlhqgcf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2npmipeoh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vfwurqjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbzlprdv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uptjrhdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlvuifzr.html


<!-- 参考信息 -->