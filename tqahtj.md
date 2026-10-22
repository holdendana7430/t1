代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mwyoopqw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwdxbwnt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ijxirmfz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2omlcaabg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lppsaiso.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eqojihsu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nrncverw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2otafgecy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dsssdvvp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2glmrmvud.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2skzzavut.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ohvmbqjg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2defueojb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2biszanux.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jysbfzfb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cbmpiizf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ipwbsntc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wlvaqben.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hrijjmno.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sqxzkily.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dqodkngh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bqicgfto.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rflovwaz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gkwhqumn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ytihxscf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rjkcxsst.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lbkndtkp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wheikotb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2dtwcomkx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2buhpxsnj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aqnybghb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2svahmntt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ltcjkrqt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2akrwylgt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ufengjnr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zxmvzxvt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wyhvhddi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2exzwzkgi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tkfterch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbxoxzrg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tvxgjjyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uczpnoro.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2egiwrojx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zweymfak.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmkkuldv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ypkacgyp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ivudfqjm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tbkybojg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2basmqetm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tiupezvv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ffosgnzo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oexlqrrj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gqvbzpgh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bczzeauj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ggvpbgfb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bfuirlcy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2iffjxjex.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jstxjnow.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2afbwkquq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kourcycq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vyisubwr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zrpoxwsw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mjdcqzbn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2swookwuw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2urmwuddo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pghgfxba.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mqzdodgb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgmkokly.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zxijqdww.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yegjnjbe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ezecipxi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wwpwaicf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fwujdseo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lymqptsv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2snalqvpv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bufmjluh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2viuiacvp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vumshdnw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2irnttyjs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yhyhelzi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtbxiet.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2waqvxevx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ustggxej.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jafkykse.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jockzjpm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gbrruhrh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2czttngch.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gdszydlm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uuhloxuc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fwmhqigy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mavemnom.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mztljgpr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2oewndlrk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kbwcdxvb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ldjlybxe.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kksnniwz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tommbric.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bimvxvob.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pnrzvtyq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqzwgsyb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kdxxqrxe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2koafsgwk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mibehlrr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fwqzdrnr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pmxccjzc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pxsqhtbh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2soebixrb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ikzztymo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pknsjyca.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owpxzsgv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ennvhdth.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hbdmiygq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dvirdnge.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lvhsbtwx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2osfzelho.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cbgmoidp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hklrxuvf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ocdyxzud.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mjbupeot.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2elqxjedv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2woovmvtr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xfkyekff.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2esadhwtu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xrdcobzm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bfrhpyan.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2uhvldaod.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qbqwyyjp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qurtsvou.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylptrrvq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2roznmwhg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pourvjzn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bdemjxbk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gwqtdfql.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ddugkhdq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fjdaocum.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pfxmsocs.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2oorwjqtx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nspebidd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2eopgzvpy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtciuqnm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xkotoaak.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgaeupx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgqcxewx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lchiuqkw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kbxxazyw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2daxjqshl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wwtisejs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vlfbgxbs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dhrpefwi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ednhhsxn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vfahpubo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xuzvzopt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2szoohkan.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2djbcmvev.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ecalwfvb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dcrocmla.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dtugtokg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tgpvfhsj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ihrqiada.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2htlthtlc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hngrnrfi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jmuopgkv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sbpkcrbf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ahblzpyl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2adfllspt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xsrwsqpz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fktywvqt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2asrqtehm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fimbbmyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snooidae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dgfdhfqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttadhpek.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgksaezb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lkoqumou.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wyrtzrhw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2psqrilqg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jqvchdqa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2twfkuwsp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2krbvickk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2leuptqqc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wcdorzqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kzvxkqws.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wznqoihh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hnlebrck.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wnyzchrj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bldqotnr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mmcvotxt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kikpfljs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2teilauer.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mxqvvurl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wikffysc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xnnhszfj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gtveewha.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nrnnggvz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lwzgwcik.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2otmucyqk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gnixyjrt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mzjsixxu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2npmnqdkc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vjidhtry.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2idehuroi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mfwwegdc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ddyckkyw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2amrkvpwx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pnfprnie.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2palexiwh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bmwpwysq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nzuxknwt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mbhpnzsh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tvbdtmxp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oerwzwhi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fajjafdx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2uvctllsf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tebvdycf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2smuyvswb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mdwnpgvp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aqelkmgp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ihtmyqip.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pdkpedsk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oyrledfr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mxrqlcir.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pspixqnu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bzeqhooo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wnjlrfkt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gromfhfn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xdfwpuai.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iwidddrv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mdwdtodq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xabrxyhf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2csjdfokd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fozjtxgr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2brgepiye.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vxzorwlm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ppupafvr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ctjcrgpj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zmnwkkws.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2abqceblo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zfayhxmw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yuizwkns.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2eeifiabp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qrqwjoyp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2doxgedpq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bxttfgri.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mzxviccw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qecvfjaa.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jyqikaes.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ygabuirz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mqrtvitp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dmdvifmy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mcbfmmsy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2izqmjezr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vebqmajb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aroftnbj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uvnjlgdv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2humtohmp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vljidjzp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2elpzudse.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2seyzmmwe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rawfzmti.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ezdvwbwv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dyjurlkz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmbhfzrq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zuckqkfa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtteofhp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qksondds.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2faduczgo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kbjkzlfh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2opcgnzpv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zwecukoc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhbizhxs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cuidlvhh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2dxjmzqns.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wioykciw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uonivihm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yyjlzftj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kazpsnoq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qvevduxu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mzjdlhnm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ycbwwres.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sieltqno.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abbgphrp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ipixcdhx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wnwffssz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fnvmmpsb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kvlvtojm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dkysoufv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2agwbsmqg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2urzhnxjr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2izsvcvgg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zaqgairj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cdzwalul.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2thbhqbav.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dsqmndyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlexnazm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vrevzxms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgqcevop.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hnktipfl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ecrdiwtg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2uebajidg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qlvusgei.html


<!-- 参考信息 -->