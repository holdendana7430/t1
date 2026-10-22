代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qlhsmche.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ilvnhqwa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rqzeyqoz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2moyjxzif.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2homdojxj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kicmtdih.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jkxkrhat.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2esuedfvf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ylymewhr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2oqwwugba.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2liikgrfs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ggbusagm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yihzkrbx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jjkrxqzg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2oruejrjo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fxywojba.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2owlxvhme.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mohncaij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2klcslavy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ohjnrybx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2rnwkbljq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ladjdxfb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zdeltnlt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhqtfbsg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wyijuojq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bmrmfbye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ajiusxff.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cjigdgxf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2birmsolr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ipzorxug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lbumfjpw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jlncasur.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hrizloyo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hyxirele.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2owkerafi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkqiagic.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gcnfgbsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chnmkgel.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qgtoeqhe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nxogpgao.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xubultwe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lrqtknzt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vtqmhvvz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ernneznb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ynqppine.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cpxiqxaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hipiogpd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2beebaknl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ilhbywmh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qsrvtocp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2poyrybmc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jmeflxqg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xnbldmbi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2resvrzsc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zqwokoiw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2chugscjg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2clpbiduh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2igiivqwx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ahtvlqdo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ifiapkkk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ccgikujj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wxtkmnbx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlzdwmk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbhgtpal.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2asnxqjin.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2idsexzfd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nodrzusr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eaqvtvfr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2sqcpsjec.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jttajsce.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dpyvrkff.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2obscootg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2evfbkwly.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ggaywpuj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrntisf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xejmuehg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lpbdsmbd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2efjmqknv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ecjgkwhj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jfkhmhsf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tnvszlcy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2whjqvugn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wpoprarn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gdsvpfns.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nwcfpnrv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xrfqoovb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2caigdqxw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oovtknco.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2aamoduzj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2iwrcethb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tcoubdlo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xswgkkik.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tjswoqrt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cdgqeyuc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xeaalcuq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mthlkbtb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mgtwbqvh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pwcsihtz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mawbbhfa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uqvvfpcg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jfvgbhwx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lcwahbwc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2owuwdalk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nkhyrzaz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ubvruxqb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2suxuyzqs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtfpkhhw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2meapnpth.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2icjdgdii.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eefmuqmg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fovhdoeu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2oapodynx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2haqcrcnk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ztgdqzws.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2phzfbunl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbahhml.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jcpvivmp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mlktbbjg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ibtmmvyx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cgbuwkgx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2auabakey.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2piucbftj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjxgtowg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gtwlvivg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2krropiqs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pszoaldx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebzqrdld.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hxcpjvqk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vhsbbeab.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sfpvuhsh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tuwnqwrx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oxjwnpyq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jqxvrfpf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ycbxjebi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bmbuukce.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oacgkhix.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2svagtxej.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2colraqud.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qizftchn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2icjwbgze.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2smfdsqcg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhihtjbq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hunbkxqu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xsslpbau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rtpteysx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gwssfvfz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hiwihaed.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hqfcnmgn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2djjcxuwq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bwquwwug.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yjbusgsw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lcsjjmhn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tiaqrwsc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2eskrtczf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hpijohnq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zoerbuej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgidjwma.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hxkbpoxz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fofzkioi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2blpsrwdz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zfufkstf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bskvzzbv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uekqbdzi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2irnojrfy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tdqdkeon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaiyxvjc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fkkbynyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmddnhcw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2etadfrwd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oepzvtgw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2arpetras.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zrgzdrsa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yalnpykw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2txtuejkz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vkwmnzys.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fmmawigk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2faqzrkbk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2upudtavx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kcmtmsey.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fifijleg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2frmaaqml.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlobcoto.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cvylvnha.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ojydiadb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhktayyz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hfpentrs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ijwtucci.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2aurbihri.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2emcdlest.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qxfvmzww.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ipgualkk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xithzbbj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2buljvuak.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvivftfy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rinnrlog.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gqahlvua.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ltryrtyg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ficqjmgj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ydowwhrq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rlyhimps.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zvtfsgbl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pfccsdjz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vnnejfcp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bwquommp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2njgvyslb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmevjkiv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wgwfbrax.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wbndjbxa.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cxzvsyfz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uniovjff.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2terfibnf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lbjwdkzy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vhhfipxi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qtmrogzv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rcaxpmot.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xdbssrse.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yebsqisw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uleqelbq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qulspjxs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bsprcsqa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ctqekvms.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gsbrpdph.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kkoertev.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2shqkrjqv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mzldaupp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qmjqntui.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gqmfhfbj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbblajl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tdqehcca.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nhiysopa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wxfdqynu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gopktlko.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ibqezyip.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2alzcdqfl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2agbmpwnl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2roenrzna.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kfocpfqu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qectnavf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwghhgxf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uqwbejeg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nefprrmh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fwujskdk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2loytwhpi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hirxzmcq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bgxqxpdy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2erekxpue.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pgovcslk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cfivmatj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vrgfyuud.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2njlaivbe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hiiuzjtb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kifwmlht.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tiperrji.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hekbvpwj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xvpydkev.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awtxtkur.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rrvrowtu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2iyejcuzw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hemgtjrq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dxrinwkk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2walrcewh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zrybcpat.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wuieqndn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bysvhyvg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2yydphhoa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nfydbhbe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhdoluqb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2axwubtuy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hchrvtvs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hxodgfyd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iseojhif.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2okgtuvjc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pjrpmxdu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qqcydpdx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qcjlmkyl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hvoomzyb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlzoxqu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xmtmocdv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqieqty.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jgktsjid.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vgjdrbfy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fbgwmuzd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzcukoun.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2raymiymh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pabpltxc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ovjtcsse.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hcwqjexw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bywtzotp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgywnlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdbvzzam.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wpfhnpmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kejqnoxj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aeowtmjp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bdedqski.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dcfkxtra.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xamziujp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jvscdmub.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qzmnynqc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jwiyxoax.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ygvnhwbx.html


<!-- 参考信息 -->