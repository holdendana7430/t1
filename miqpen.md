代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zoxhaqvc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eotoesmc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3knocdieo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3msftsmun.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kfxksmxx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kjtoohex.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3aejkrhio.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jseiwhsu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ssejlqyu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3klbyvweg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hqpgcpya.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bfjkdukl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3clnfulvz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3piokbgvk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vtbcwvst.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3odueiykv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3etjhsyho.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rapjxiwx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3itslbcns.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3uwdiqwfv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nbmqcahi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3guklzmxz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dbxjmiya.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kezdvugd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mllyficd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qlhtthkk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eijycsfc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ijnfhnoe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tisdujuw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3smsdwppk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3juavzgxv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mxbmdllu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jfbermfr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dlfcrzhs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pchocozc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjkizhjc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ymtttxcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrtzwknl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzrlgeuy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gupbannc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfhnhopw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oppjxgkr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jcknannb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3muespvcv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jnkyeihs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3eftzqxja.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ipreazhk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fpgrdvfi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3icmvlkfn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzpugbnz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kyxcapna.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rtdwjnxl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dswsccem.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3srzbglws.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fqrvvqjo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hhasmekf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jdjlsquj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dspxcbnw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3smnlgtji.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgjeznkd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iidtvpqu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ewlfztjt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yhzlbwnj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xshihwfo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3umgadacw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nfbhskln.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hewxxwdm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gejqbmul.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vtdibikb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gnoydgbb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zethyxam.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gifslwlh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zdhfzffe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ijywyjbt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dvmrdkim.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vfmbhxak.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hrchmrgf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nlwafwul.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xbpjwfpp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wliiuerf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uwpihsuq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ihyfcsin.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hykrcqiw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hiygmivt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nppzoizq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hpyvdovt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yesdcrcs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yiyftpgu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3djhpdzrk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nxqbzfqm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qnmglbwq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kjxigyei.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qlfbhxuf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ltkfjpfa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uypojppn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nnmzdxwc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xzhrbwlo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvldmxrs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dkpeikxn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3btsktyzl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3otzcxwqp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qatlufzz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kzeagijg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uuloqzgf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nqhpbkoy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ynwiping.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aomvrsar.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3auidujpg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3suohkogy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ayrbbwhi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sjwvjbgs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ajqxuser.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3koshoios.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3grxdclia.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lvqqathv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3udaodvul.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3eywucofl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ogcrolrb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3webzjhhe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ojotpibd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zvvkdrgs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3stfaqsip.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pkimhbiy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3sjzbxfzt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fjtyhlxf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pnrmlhqp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgstsuym.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ewrtikls.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wsoycoda.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qvfdjovg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3eqwmcuza.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfompyyg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3irwaprel.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ohwigghz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3erylfrxc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mepampdm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwvdbbup.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxwvfgxt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oijlwnrj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vayfowvw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jkyosque.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jsmlbmaw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ccfbpzdn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xmdniekx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bamekgqt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eruyytcu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gfuleucr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3spdhryfq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugadwdhk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jijtaspv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tcomyohy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mufolqgb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nwslkpnz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3trpzdpxo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sdnukdpg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ytcrqhhu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gopbokur.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dypufxji.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wknersdm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wgiualdk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vltnyzov.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uqfmngia.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zsqhhmco.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gnduccqf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ztqelzfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikylubtg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3iunmxdcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iujcqsom.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pqnlukwb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3moyinzbv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gfqbmhlw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fpjzzwrc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wjjvocdd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rgaqlfgq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ybyddcon.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jnwvpqla.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zfuyikbg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yrwwiurq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uisyzmcb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kgcsksoo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ylxrsfrv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rygcuzit.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lzhvtkco.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nfmyhigq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjlbgkbv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jwvwdqbs.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3drxwlsub.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pvzrtpcg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fnyolhwf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cjqfflfb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jgbpvvvc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vxzupwov.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gfwhwegm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nupvdjfg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3feqbndgl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ngswaaoj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kgkenecj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iydhckrh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vvhfopzc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eakgbfut.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pckqlpfe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cvxzqvvv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qtqvjqsj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pfhxsxhl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3smwthayx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbktftvr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3efrelsjo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhdodzb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qbdolwjc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gudbhhkr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qkdcrwkb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kvkqhstu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3sqvlfois.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3htnlyruq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ilbjhksn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzcyedxt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3watwvztl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jpunrleq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cktsclrc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pfidosdd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dartxjpw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zksscxvg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rtfmiisg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zgucssbj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lpyygype.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nlfdcxsk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bivlubvz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3argwxsvw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3svpphlwh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gslpbkqp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3iigbauvo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ausgului.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3erbcafol.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nidvnyku.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wvrkhmjd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hgrueiwr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zrzozxgw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3oyrpbwea.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcyuudid.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fjkbeuqk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mnfdjopb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3szrtlqqw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qnrsoqdr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3flkrazhp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bqouhxze.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ubhstyzb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pzdkpmzg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lcgxrfzu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3crgxudpe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zgtqopsm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3epsmijxz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vvlvgnvz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdagoloc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fgzispyu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pfzpcyvo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpxnykmn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xgjexacp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zdguqeua.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fwxkfvoo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3muaqebll.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wbyxncsg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yydhtdvo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ecqzilzz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jzjzbevk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3znocxwog.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3izfmcchz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvuoezki.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zmaxkjdz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnoxrizq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iybdjmva.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ysrexvjz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcxpjxao.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tfiwhnrz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3edjufinz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nbeffngx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ibagqulk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zpaqyabf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yduqzkwo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3raaeqfyo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3oajohbdp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dyswzaea.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3segxkjly.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hilnwkdw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tqkgajoa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sipmwgdy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kuxnxqcv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oseqfogz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3awnokjmj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxycvzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taxhzipr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nhpzkkod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzzahnyg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jaeujorf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tkrasfgf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lbaiytes.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ngdcvobc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vntbafrt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fkevxfes.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3quqqbliv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3adblxzfy.html


<!-- 参考信息 -->