代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hnbkmvwn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xylhznok.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wldkegbe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yuqwxkdo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2saklcdmk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hgrlrzhq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iitowzyw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tpaeqiyk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2csfnnaxb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dqcdihxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tcywhnsz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vgszcbps.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ruwwbqvy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yxgbmqcv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qbommhna.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gmwdnktf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mwnansix.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zrolvyak.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kycsraco.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jplwhsni.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uwiilmoo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gqbomhsh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uydrlokl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yjpinvkr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qsyszcdd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dprhayxh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jgjobzdm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ogaywqjo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ismkxsob.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ncpigetw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2naguhcma.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rdjmopmz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoeljwvh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yvzhnqnd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2metqlpxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrcftnsp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2yzdrfwmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spchnsnd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2daaysdiu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dzlhvkom.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsztfmvo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bnunqbgt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ommitjdj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hsjjbnkd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fflxaumt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yrfpncor.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kdduogsh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qeicbiuh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mmytirls.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gkvaldly.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cmurelcl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tlajkozw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mkzzlpjs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xuwqmxnr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hnppbkqa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fhojrjsn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2glhjodjs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qqpxywdg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2krsngyyj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2asgxykqj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dnkonnqx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vkimnuns.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2snzhfakh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wluhirls.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mmmaehlt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ecyfoxke.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fzwkiuhs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2spzffspj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vtdbrbaa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pkcubovs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xavtbjum.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xcpaffxr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lhlgtkcl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lesgwphu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lhptarpg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2inijfhcb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lgbdgplz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qpkitppn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jzvncuqz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hasfuqwb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2foijmkla.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2whvkeahm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2osdehdjn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vvefhpzs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ljmmfped.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2avphzawp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mbsjjtxu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2znpfebtf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2oatxhjeu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zlkwpyxw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wbkaalsy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jvmzgvdn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zrwggwrt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jhzujgbz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2prirgtgl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zsqjslsb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sdvyktce.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfdegnkn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rbijtqil.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qikzruju.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xrzqpzid.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ljgiaktc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gbrfiejy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qdokgkts.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tdvsgcuq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwwxdbt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndffmcwp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ipusgepp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ysgdaemn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hkrylvbm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ocyeqsdq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2imvxldso.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2prxkbwfo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mfsddalj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dtgwjxdt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cjwmcdwx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lkirxolu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpofra.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tsivtmzg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tfknmxew.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pzeujmaq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2usrjehxh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ganpciap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bdcsidvj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2illazdul.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tmtactuh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jiaoyimx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2bjkvkjgx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hbuktemk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2czicfhlb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2upbjfdsy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yfxzrsgj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wcylgvek.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rtgyvcgv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hmytcthf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rezwqyni.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xegxcxyv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvfeedoz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lujxkaag.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bsfbehyt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jqrhvehr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkojooxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ifqlnrbb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jsnfxsyg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysyshizl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hsiemspp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2frydesvd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wjqsybwg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fetgskot.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jsszrlwy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cthtiaxd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2acxnqman.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vswdqwnx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2utlomelj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hqbvsjsh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ufcznfeq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rlefyghc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2snwoltnz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tdrhobwc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dhhtbqiu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxdgppxc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hfijlyum.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ezezhqrm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eljwxjii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2alkynzrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usgbkcxv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ytuczxmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkpzxjry.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ovwmkadm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kuydyjeh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ldhdocgm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lztgifxm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kswwcqrf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qkoceicz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zhvfevyz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dpncewwc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2whonilmy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ojhfvfob.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fmztsizz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vorhrzab.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eygiztlx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwprojlg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mvfamyij.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjpokm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vbiwnbpx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uunulfdo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uxtexyod.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bvbrkfgh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pfzmheco.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xqblfdpq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pelyefvu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dhihybtm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nnntjagb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nagljxch.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mwokcyug.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zccxsvko.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gwcmpawz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yjrnidnq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dbfjhbat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2snnitdch.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pcpyzbdn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qqmlxrfp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2apfeormk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2krayfpdv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kuqjadfv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jazueauf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vzgihsgg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jwngtili.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xqzlzsty.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ksszjcvk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zrmchovr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hvxxbhvh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufbcspzb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2keeqygcc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2daddlcis.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zcncxovc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xfnclwqy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2clhkgrdt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ptkjeuou.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ivirdnxq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ypdrmztg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tsafvgbv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iwrskajk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dwlncdil.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2whvgbadg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2haqeqkud.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tijegjmb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tovggmfj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jzirksub.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kvxvitlt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2spdgkchx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvvmpcbf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dssucbhf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zrsplbcu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rfatbckg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hqtzfzue.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2oyrzfelg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kcdiqwmv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wqbobmyk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2cqnigics.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xtmnybyz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kmczbpyb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dwrngwcx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2btaqgiyj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gvljjgoe.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2imvsprot.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2udnjgwfj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hdqsvfbr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ssualald.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tngevvok.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2sesxslrr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbngcyut.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jrpcbwvi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2joefztxp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hvnmdjrv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kzhvieeg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nvmqepyx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2atpyzptv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jpmsdaom.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ggpdbpfd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hvxlvjdk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qccnfcwm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bzemivbd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xkpyzvxl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2edwnrdzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ehxxwwyi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2acaslrdt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wdsvgazc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lhsmxhut.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xvllheei.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fuxexuna.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yukgjfin.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sfurmzyd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vkgirkyk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2puvefdbe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sghxpoon.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2pdapohan.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xwxutdsh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cpyhnoxa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2eymjscch.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qjsbrttb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kmtsanlc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mevixvsj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gnvtzhsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lwvmltln.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ethhermm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqdjpho.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tkhixusi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vgalxvon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgfjghiy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ufbguoxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deyklzrc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gmauiqvh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ffiycpel.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2onjvqwtf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cpippvga.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cysvtbho.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2wierxagj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2agyzmkhj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zkctewrd.html


<!-- 参考信息 -->