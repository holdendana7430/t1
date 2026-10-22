代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2voalmeha.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oamduopk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wgjzrgrv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2aplebdcp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lmvxqqas.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2woovygtq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fxgcetfk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2briwfmwq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iogfnhxl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2juuvxuum.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2narapgzp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rtfwkvab.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oznbjmjy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2umaqozwc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2syxkoagt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tgxunyzu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xdrpdpct.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mdgbautz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ousivpme.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vagvwixl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2paioeppr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dipbugyf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hsvttnmx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hnsjwuah.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zwfgwmsh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgmkjnon.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jwzlgucu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mrannspk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2aiinphff.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ocaauacl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rdyswgvg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ptlxyntj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wefsqlwt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2twyjujpo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pwlvcucv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqtcrjlv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xywtxxzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmkosanj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mabzyafx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wzzdlsmr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2trigtxsr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ppeyihdx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqlgizz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rmaxdufi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2upchkioh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ekonnmhr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2aqjoncgq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vbmgmbho.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhydlve.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wqyfkrsy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ducodyio.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ijqqowip.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2obtvpkki.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2grfffjih.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xptvvqjr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pqsldwkh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vehkzvgw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dnqolrix.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gugsublv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgczumpb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bqmscddb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2llgrjvbh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fmqliadz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yfgzzqqu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kecutysn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xgkcddbz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tamkutmi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qfosinuw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2atdhzbfo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ipnvmcpu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hokcoije.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dmzzksyp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dqmsrinm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rhoguodh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zvgzcbmm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gclpnakv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2phxldnpj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2emizvdnm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zpvgkcoe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cjabbzmh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gckuuclc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zlzslcoo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wtdzfshd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zrquncfd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhcnapu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jylezqgd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kikydqls.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2lawggwrb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2azcmkuws.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pcenqxni.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2taeinbgd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fllpbyjx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ucvuigjt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ulsgwmmg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ttflxzfb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kekfsbar.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pfmjmstx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2szhghleu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2facdhfys.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fvreejur.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mutcmowd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jlievenj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mfsxgezy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ttrnrzce.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fusugmmu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itglfnjm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2opymjhva.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xvywqgbz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ncimpojr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jedlmlqd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2olnkzxcl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2riexptyt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xycmqncv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nbpkskwk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vsbdsama.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pyslvmku.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fvjaxdih.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjmghabi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dsemqqol.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dscsqqnm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qhlrpzze.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2iuylbrvq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sokuatum.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hcihrfes.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kgfztnqh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gmzpgfpe.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pasgtpfq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2yxykmjbp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2padnxtua.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fpoknxwm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lwbbwzrg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jfubjcoz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2afovwpvk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lrfvgbby.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vbdrrjrl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkbmwcdl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zkkntfda.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gawzdave.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2otedrhxp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qaispies.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qwroghoa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2obiqqmcm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tvcckpqg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hplkdutu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aabigjtb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zifoixea.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xtnmdwqh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rmwahxpp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnnvhrvm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zcfzejnc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bwcpgcik.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uuxesvpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mihuoxaz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oasoxrxk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zomcnrut.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fqpbyaaz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2axuhnlly.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xdwivtru.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ppotsegk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ddfyjobl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2taxdfnzn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jgkpgckb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yswtdvea.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ctcfdvaq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2splanssc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zglferil.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2udoodmzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eixifqwr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qcakrxji.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ziyrizve.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgjujpuh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wmvxwhie.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xswxhuwv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qznnqkro.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2luyorzye.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bxxebtob.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2khxgsiwv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vsullmcc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oxnalvnj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kbrnfpxn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vvmxtwgw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xezmuzib.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2amfgfqhn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rrzalgjz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tnxbhpja.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xqnatuev.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhymnenn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tdoqehki.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fuepjusb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nentyzsf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qsyqemqa.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wziovdff.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2favgnznd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mjnoqlsb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hsejtchh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wypxncjx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dqujetvf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ldssczft.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvcbpdre.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xmkjlazo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rfdhcady.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gmauicea.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nfdusirz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ebrauiec.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2niedbefb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hafhhwgu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fiyrueyw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2efuvqtef.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bcemcirq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcymclje.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xvbqfbtd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hpuivrdq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wtpyjidt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ylycwncl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cholqlmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nwnhtkdv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mwovdlxj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2napvpefc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uonilmhx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ahtvtuxg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2oahysymh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zujmvbmq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rydynunl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lsnfwvmv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2braknlgx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qnjciten.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eqcpwrwz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bgmwxjty.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btdiquio.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ipkfikcq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxtpjtpl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vtthyhry.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ewjpzyvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fgjfyfvy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wfdmfmsp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yvyyhpgn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wrvctmse.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fiqhiife.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnicyjho.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mlxjfigg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2axrrigwh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gkjypxer.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lyhpkbvn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xbjomszc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wzpqfloh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xpmajycs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nazuqulx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vmukaiap.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2krzqetfa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eaktnpaz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2oshzxshv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fcokgjwx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lhrkgxwl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qqazsumw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nffplzpa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2khikdxou.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2sphufonr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2grsketze.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2padxqcxx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kauvissr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jllltjzr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwstdhlm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hiohkkkg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ryuoojhs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvrdktqi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ghryodlb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bynwtwev.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hntvtilx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iesrffbg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iltedbev.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ecfdmuey.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zpvbkufm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ghshviwk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tmweqdyk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2atgfawmp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xtsdgnvs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwaxkzpc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cftwtxcy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gcozpkjl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gfbuvyfb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qfpdgzrl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cjnhdzqh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fvkcygqc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2obhlvmjy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hffvokfe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tlctuugz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kmsgoqwb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iyfeguur.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ulchbica.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wflnrvmr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2epguuigd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbujyfdv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ozblteog.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hdzdmjlj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vgmvsmtm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gwrenzgf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jjmrlril.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2deqblzsl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pbxhnjyo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2aegesctl.html


<!-- 参考信息 -->