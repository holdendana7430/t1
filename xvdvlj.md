代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3uzenukgo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yrzvgpbw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oakxlryj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3whfgaxqd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vjzctwku.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iymhwila.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nglugjax.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mtevohde.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3efuatudl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jldfnmou.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zirzmxpm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kwftcjng.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3brskerwm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ukvamfdh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vtplwpza.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rdyszaxc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lqphmmjp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hytpsgxc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zxadyizp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qysawkhz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jfunkdsj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wqeakrnm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gghoavjx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ekfhjqby.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yyskjprz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrxuadth.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3llpygfro.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nwshwvcw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ekgmgtyp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hivcgqpk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fwpohnod.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oebjrehz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3udgvijcj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3alrqadcz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iujevwzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmanarak.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ofpqbglx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyeuvtol.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfiztysa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nlvsntzy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwwprcwe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ioluakts.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tgsejqba.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nwxapllh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jczotygk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3alefxteu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3okrjnfuk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rmblggts.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihftaljo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3omgpytix.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lcidkyxk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3llamnzfy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zfxzbqcw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3umjpfjtk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rpmhfitf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lbqtlpja.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jvwkkwtz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3auwqvyey.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mqgkoigq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hbqimqwu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cxocecpp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3thytslmy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iywyoiew.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qzsqoupp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pcjkojno.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pidpiscd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lyuipold.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3sllwjhea.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3yjgmuzmw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nanrjqoh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3owfzjmqp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pdddxzmh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mkdwvpqq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kychrwfa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cvnavcso.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3grfxleik.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmbjibb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yrgdftbi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tefnkcix.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kldeobrr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3trpneium.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xmcwqdke.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qbanzbdg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xqydpldw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fxgpzsle.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kkzldnga.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kpauomvq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3htkxiwdk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3labssnbh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3spwzflja.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jvhlqxcn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3imzfyvjj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ngvpnirg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aoiaktzz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lwzkpxjn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mjdozfdk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vivxdcpc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgkjdgzj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pjwqlavy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3oljotjlz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3brklvekj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eiufkwoa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lipnmjom.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3apyjgdam.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uxrgsfzf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqsqnscx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3clfsztyw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yhdnvwog.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xmtuozqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nrqedpuu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lomdrjqk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eiivlmba.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qbbfhpyd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ucdreabt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tyjupcci.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ygzmatem.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tcphnpmg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ankrvxro.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rjypabhl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ydmdgxil.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aipnejon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wlciivhz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oidcsbbn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wdwohiga.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eqaiemjp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3erzhlgvc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pvsoflmr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wkjwwfzg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xmpdwjyq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jgxtdexd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tmbghivf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hqxfvrcn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uaowewfq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qdksuqqk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3unxumrmi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yecaumva.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xtxlmxrd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jpzqdodj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mzrhndon.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3acuhsiuy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vjgjlfgr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sjxdmwme.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ymejzwno.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gbazajor.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3covmjvuq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3afocabtl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hlkmkpzv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ekkyoonp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fmovvrbi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fjgdlvqd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3medqqxsc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kymfdchc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wwknlkdj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3phrgaiac.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gnrlewsd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cxfvwonh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3eagxalqa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nvtxffgh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3easzcjad.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nqrcoavv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3poltqyjt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3becoqrax.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rdhbgpqp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hkxzmwpt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vdrcsmey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hatlfbru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cqhqyldd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bymehlsp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3amvpcnxi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ghiuolkr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jvzuhmyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uqeuzqja.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nxjoclsd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wrncvnft.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pubqbujk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcligspu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3upcuehah.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cewzhbpk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mhhoqcez.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3npqrjzdf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tgqcgsxn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3acwcprda.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rcsrdxbe.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3apndajun.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bwzrloxw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ikgzyukz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3luecsrgc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sdqmawxk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3akgwihib.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cwqtlgqv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3psgoovpb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3heiiaaoz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oasmttnv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dllftlhz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pvexzuvb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcxdnkd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hrxglhap.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nyjtisvm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwvamfuk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3swjbypca.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gfptrwmy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ysulidwc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gvwxgwag.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xotipugk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pcpzsmmn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rtwtskyo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vhmguins.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3preijsgt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rcwetqiv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cmjymebp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3iaytsuxx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3purhzhir.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvvpteeo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3psyddumq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fdgacfiy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ooqiosuc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fjaepqwd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3iaupkfse.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aetocecq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sgsebdgn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jfgzqcwy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vtjehzhx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wccazelz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ovuyypux.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dhvkdirj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kyypuqsc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wutpyqoe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hjwqbuqw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmdhxiyf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fftytfnl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jynkmaau.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zoiblhyb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xehmmfnd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ievdsgtm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hhublptk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mkzwngne.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gjrjwvgq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ablkyaew.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mmmluujm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xeyxujoy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rbztjljk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cilrklub.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dyufzajr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3btvmirif.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ydmawvec.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3roevaarv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hbjezeqj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gwtgsbxy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yyyqrgzl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3chwnjxfn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3srviqdns.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kebhhowd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fpjupaqr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qkwslrtv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lxfqddwy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fykduukw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wlovndjk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3urnntixu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kjnssnxz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3alqqhber.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ozvefpli.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3alhkzxde.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ptmvvjbp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uqbzpyaq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3obtdnhzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eetnfiwj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qffbxhop.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rbzomval.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tjjtjgha.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wsovpkkv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eoevqmpq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hkyajdgv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fiyhkagp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qfaegepn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mxuwyeyk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jtpjlsjz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbckwsx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fwdcsgnc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3legwvkeg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xgxaazxi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3orawnozc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rceqricr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3upoeeubg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3itxghxtj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wwfdvnpa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ztoewkcp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzekpzq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lknobxex.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3utpkjtqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3saizsexf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bybbiqik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivzsmqjg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vegimpcb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qeitujuu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rhigbsvg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezdzddmy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ogucmfcl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gnwjcjqa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wzhimqzx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jtdqvjux.html


<!-- 参考信息 -->