代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2nljrbwnh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ryrxhula.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mydfzljc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bjufkici.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2awqkujrz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oajblbaf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rbjlpnlo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2enlqgpyt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zhjufeep.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2upvyxfbu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wamaocsf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cpfwdrpg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gcshrjap.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2unitknti.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xxjygopq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yvhukixd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzpaxb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2uoghazmj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wngewuzn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2myjcauhl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vvjmnozn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wylrrbmc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qewcefje.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2khunyugp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jntzraif.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qvgxtjzf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hlikynxy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2roejjcoy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2byaeprei.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2oebrlvtz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bnfmjpff.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nowzvgms.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2osuxeqye.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zythryjf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sonmxvst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsjgaeoo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zxbrqufe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gihnclps.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zbejqarp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ryhednut.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uogukzzn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2afzkifth.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nqctinki.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mvgzrary.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dktmlzoz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fcrabcuw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zlirrjea.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tusburoa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2guvhmqbu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qbremmfj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vwchqhdo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2atjykzaf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nrbsbkfe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pxbjlyix.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2oqgsoyem.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qydparak.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nbpdymay.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2otfosrre.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rryyejme.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mksiisoq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2djbjrpup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bniinuaj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gznjpiin.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xcomvmgg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ptwumrba.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2iqpfascm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2irlejqfg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yooixcab.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hkqowkak.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xzdvjtip.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gxppvnsd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yadbarcw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ejflvvsh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pdzwtutc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gpmpodsy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vnbmdyow.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ttgpnezt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pluvkhfc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2auobtszn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kobtfair.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lpbboczr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lmknacdj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fcgkakri.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vanurnla.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qywmnmbx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vxnyrdkh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lnlhkgdb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2alpdrzpq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nsgceiga.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2siijnqud.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xnupfngh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gsxxludg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fdsvnabc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tosizqpr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2seasdtmw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yglmsbcm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oadqsspz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wgavmvqj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wofldnyf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rhreobcw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bilkmpnb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qwbmydrj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uvbqgqur.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xykgdawp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2afafimat.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ambnwavb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mycxuhme.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nycvsrrg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wkhlkvgp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zfvrfoxr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bwkssdry.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vrqlqblq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ruoqjsnx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2atjcgkqn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kvesoeut.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtfkfyko.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zdpecrsl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yfbfkhyy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nyltvvyx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2olzkqfvi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ljcplpyx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vnlkhneu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lffjjdnl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dqtprjuv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftdguupe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tyzdfbdo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kcagiyot.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sueaxbku.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2agizohwt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2prnxpgjs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xpgzqsxe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdxxbnff.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jyzbycyh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2eczazjon.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ayspdcih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oarxxxlf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umtisnub.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkuadqhw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgioidvq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dkelvrxn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sxknetqt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nbkturri.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ivpjoric.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ugaavhnh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2luldkzhe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lacbjkzu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fqjtuqaj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xdqgyodh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2whavfjha.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2culkbemm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ffkatkds.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ahhkcljq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2icerchkm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2phybbdhm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iqntiakq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uquvqczu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxhqccbb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cpvdfgfc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mllruvvl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uvpkzmmc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xcafmudw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kwzollcj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qqbxrfpp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sgpwywap.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hculgjqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vebfllaw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zmiwqnln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loaqkhqd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2idwxihdn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nytzqrbr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ladkhghx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xueghcid.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ovzitvnk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fnabosva.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jixoiwwd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mlpoaxqz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2helhuzzj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tkfazdlq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tuavvslh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sisqqwwi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2luikoljr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dggyyhyg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vmnlpysx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kjrunvps.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2osvwkbxf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bfqggend.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zivptxyj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tbyepsjh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mzjzwakv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tpomuvdb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2niljbzdl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xwtvwgcq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ekyqmhdn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zltvzwxk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jkvpfydn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gefotwrj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2rgubxwip.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hwuwskkp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2krpgptjw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rpyajemc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rmuclgjb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lclumtxd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vwbltrvl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xrgutmzl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qamfswlh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bkkshggw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gqikesbm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rqymxzam.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xzpvletr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bkueberp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zibbbpsf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irfzfcox.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvdoeoht.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kpqwirgl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nfyvwjbg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vymhuelb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oqxgwlxl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hthqefem.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cndolrth.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xaawwbxn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hauvvirb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwboyrhb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yqnqcpzp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2riahzszs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nixnsotq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2karujctj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vnqbtzxp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhioqyz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yxemhvon.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wbxaplyt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tptvaadq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hculfdzh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ylbvbxag.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xgymfvrk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2inhzrpsn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2nilphjsy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wrnurqwm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jbrfrbpu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hkpusbar.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2voyohrxb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iievhpbg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uqqklvwl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qfbiitrm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tkjtdmrp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kkvofgfb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yyiphaiu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vkusaorj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ujkfozwj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kadbqjsd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bvmarqwy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rynsifwx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2eelsddpb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yfcjbmvv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rxcdzlly.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nigflczi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsbcojis.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vvaolilr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tnyfatma.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eavldswr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vdujlhem.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fqzmlilp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybuiqlsw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sumhttpu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hrshdrkp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmdaoevn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nradjpxs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2agcucswk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2higxaujo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yetbdjrb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lrkuvrpb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oryvptgl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ehzohhzv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2owlehhib.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xrcvlzwi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kjcxxarl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cgfffeib.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fiwfphhn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kiymubtd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2awwwfjdi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cndtsski.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xjqmmpso.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2psxxaepr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxwcdlrj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vpkrkydt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hyhwtcxl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qxwuadyc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fxyhymgy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ffuikvfs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vytmqsgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcconlrm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hkrmkmtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geqecbnh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eprquios.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2msotewzg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tijzsrse.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ucqxydee.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nbbiflue.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kmqqjbxc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yhmdgnph.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2idkggzlz.html


<!-- 参考信息 -->