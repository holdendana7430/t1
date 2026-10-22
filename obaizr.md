代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2eovpqagz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ytcwjmnh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgmtwuzi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xgnjauvv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pxklgiza.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hggvvzri.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mchsiylq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xnpqvsbh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2schijfii.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kheqnnjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wdndcbld.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ghvsdssk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jixujsaa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zjicsovf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xbexdugy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nhmkeosq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yzhhqhdp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qntakciw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rpmassia.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vxmuexlu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jwoutrha.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2enotbsbi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpoizlau.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wyeyiuud.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vpjcmktw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jhlqqist.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cglpajlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flslomyp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qixpljrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbttctrg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nkqrssuw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ikdcygcu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sojpnxkg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2snedizav.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zumvhbxp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dolktlvd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jxfzgrao.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kfdobbod.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2waknwurb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rlpeyglm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxpqbig.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bxmrnozl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pzzjhjty.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vlvxmcrc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uzlyqiiu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hpefiqia.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hmjybtqf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2oixpfmub.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2piriyuow.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uypuqqby.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dpasmszp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxszcqfs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xzttuvkv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ficydlkv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kfqssajs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ddtfogrt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2difdbpph.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nhwcnmfv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2toyvevcq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xyxgomol.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2unyryutg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2whdyhybr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bdblmhzs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ecpfwdir.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rdmbwuey.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uwtnpzop.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xxezzugr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfpeilgc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kbrxkxdm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nzpqqfne.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ffvezktg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jzcpobml.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2alcrjltq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nrkfpajn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vesqzuke.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2khyjrgrp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eqvzssbm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zlbkagcg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dqzrsyhm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2pcyxslou.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zozundow.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uoyahdsi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2whlrydvi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dacwpaos.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2shnzpvad.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jbhbypvv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yuagbmcp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pjjhymiu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dxqaisgf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtjfreto.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2myonwzip.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2btyjwdwq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gvfzeppc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eghrdyle.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lbessewd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nmzdgckc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2konflqje.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2birvhltq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pdzycpmb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vxwvyfmh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ydsuevsp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztojicnp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2obesrjvq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jhkuiyzh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rjxiauia.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lyjtzazz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fgysbotz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzufchro.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2trxgoxtj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xydoytce.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2acoxapan.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cdwguwdv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2obljmeck.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zhtuolvw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gyizxlgu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fmminmcw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vljmurfx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jkcedhfv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2aautjnfe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bkqhftok.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cccgnwvu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lwwymgsm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xzdushda.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fynwkire.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lrnhvqhp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kllhdeqe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dkqovsvd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lyhwocpt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jnnrkyvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nbcgwtjm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qnueajil.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2magrgpob.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pgqxwwba.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewpzhfzp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wgydytsq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xtyvhyhv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kgwwvjih.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jpwiizen.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ngdrqneh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2airzwhig.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vbretzuj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rrftftre.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2socyijwr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2naweoftv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fwelvtce.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2putnooot.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jwiunbma.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vsvupmvb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rosafuld.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2okauyari.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fryggkpx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ncfwpwoc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdougpw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qtxrlivq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uttqvnmh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ikypdjzm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dakrwpsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sndxbkvz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wcmzgpue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzkohfsz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vgpqqxij.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xgohgrcp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2oxzbarxs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qnvjyoad.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wjjdpqxy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nraljrqu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rcdvmhur.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2aconywol.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2weecmxif.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2lsdeyxsi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vvhdqnrv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cuxilufd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gqarsywp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zurrdaol.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kybirjdl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bifpdipv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wndxstaq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wtupjwlp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2askrlsad.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2soqagejw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2srfkjsbb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ogcfmmyj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2drmdgiuq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzysdvx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lcrsbcvr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcjdzsa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjijdzyb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cnqqonad.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kmqfecbs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hclxijrq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ruxodorj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cgeauznh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2nstdvoes.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uzrmxuzd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yhaynjyg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jovpowug.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rkhgfyvx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxydjatl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vpotyvlm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oijlhhot.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxgdjarw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vimvajdt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nuqbxepw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2huazleqh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvwaupmg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nowacuqs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qpczgeir.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oucyknku.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2guyjpqlh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lzldhqvb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bdowtmfa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gkzyycsc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmfuqhns.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kygjxhcv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qocjujgg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2njxrjqgl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vlqdmlup.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2riqaxgkc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wyspmgll.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qgjyknjv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wwwrjtyp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2stdmklmt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ejbwssmd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rhhxqrhx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mhxhazcp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2prtibpkz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fclqeiaw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2agcfmfem.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wnfrjcib.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pwlejgjx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpcfohrs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gqysxxet.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qzuhyite.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mndwyxys.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pfawlbdq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mydbkkii.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iffqgxay.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2yyzgvoip.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vztdwemt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2chwitxrw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2moxextfz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ekpkubru.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kzuuaizy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ihytlrxg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kxzwauba.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ihsuqxsj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rbnzjvxb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ikkvmzpq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kensiykq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddflksee.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2anfseqrs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkqdvipg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uavaqyuv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2llnhlxxp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rlfivdoq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ucrvucsp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cuazbdmz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2stwxkdpb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlyksbew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uwrnxftn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccweysgb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wltokfyx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2osdobnuz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nzouohpv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jacefmht.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kmciqxhg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ydvyjxkh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kygatecl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmytrazc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mbedgxcw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cxycbinr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kwiohbfx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ojodinlu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zclenyjm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pldgwsug.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2aunxamsv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2iipgkgcs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qibkdbhv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rqraskoe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2vdkaudxh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2surtsnbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkkqtsko.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jlwwykbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqpaeywf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mwybckxm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ufoxxhxb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2agpnlkcz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rcfvyxai.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mmtiukax.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jjnqzxlq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kjytntco.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cfquayar.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2okzicxov.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2axjegucl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2quaivznu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fmbxumsq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xcbabptb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kfcpdibe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qztiuzjr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zepqlcqr.html


<!-- 参考信息 -->