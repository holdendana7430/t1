代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xlswbxjz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qsylostl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ploowwct.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bkbibvpl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2anwpruht.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2krknlbar.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yxrnvkpv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ouwykqcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2caotqrin.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vbfqzljo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zjpmwbeo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2etybjefx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vzrlntgb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ilpcnpyf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ytugzuvt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nojvdmqy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tqzlkrti.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ldsokbra.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vckfqjts.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bvvoxrbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2twrcfrtw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jkqjlgjg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfzlziph.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dgvtbqur.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nnlrebmw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tfljykxu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ytprzblq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2sdljhqud.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2irkdyubl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2klrjcriq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tfehjimc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rosnpymq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2iatynvtw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nliitcbg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iitwbyys.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yernmqzl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fkomrqom.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bhaoalfi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ascyvtpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skkdbcbt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qjqvqkml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thxdtxow.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lgkfhxsg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2djruhhpr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ljdpvieq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2owrblejd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dvtkflnk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qqqjsmzp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cfsnziee.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pqvzthhb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2szeryxua.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ybzxhdpz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yiqwsbah.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kmqjkeab.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qltekyvv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pawodpym.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2sjyzxzil.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gdfqlsxf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wncmaong.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wzhsmmal.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fagesgem.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2omzljwts.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2klxeqjai.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2agxnoszk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ymvwiuvl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2znsnpbum.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bjtzaona.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xqnjrtdo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vjozobxg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gfuxjfrp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lhucmbnw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tegkwvlq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rtzlzggt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2duvlcvxd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jcntytjj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yqbutfzl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xzjqwkth.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mlhrjjvc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zasqcnbt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjvtitrj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ntlzzxha.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2viuitekx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aaggotbd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mdufmpck.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qypyselv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qwgeptfb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wkbvrjkw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ofbpuinq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dahbbari.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2epazmzcy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2somxqqnf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2prmngydw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wwjbofcz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2anugixaz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dmdonbgy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kygqssni.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2exbbsrtu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ztxpcowj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rhsniwvx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hggeltpo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rraidgrd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzfvgsaq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2clqntexv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rahukfbt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hkjjftdy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dxruoisd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qujmumlb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lzidpbei.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rgvtmjst.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2earumgic.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dqsrhnee.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ymwkcivf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2axyolitg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxtomifo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ooklyhwi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpwqblfs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2udribino.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfnhthtm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nagdqptz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxizqoiz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ulmkcjns.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mslemueb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jncuxmwj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vozqihnr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2eomlpdjk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2djzsjnic.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2znzcyotu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wtpawrev.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eyqfuhmi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uddkpdom.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cftltggp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sjjhatmy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yfughvgz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jrbnrgrh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xghevqnb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqaltcj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bnecuywm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2uoxllmki.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2iybednzb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2sudacfhx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2sxonbrus.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2uxykbram.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftrfqwdn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rsswhrpv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mfnvghin.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuemokxv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2shlhltez.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2aqpfkeaa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tkqkjlej.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jfkazykc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ujywftwn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nrqiqdga.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lledecmc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zpfkqrxp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qqeblrhe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kwmidagt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ljzqsppc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wjsantdx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2suqqpysd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2oqtrcsrc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnnidpo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qukkgypf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2oudbrgkk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ttcjcecf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dytdrgsv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ivzlsmof.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dekcntms.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ybnqnudl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rbbruplw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ermttoee.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wxlbvidh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2koqvwbrs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2prqwcgqq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gopbjrxm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bthvgwry.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bhixqzhx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yhtzymad.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mtmcxcpp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2acdbqqza.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mkusgqxb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ytptcrwq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lltssfbb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xtuczxtn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oaimrlvj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vknyfwad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsiycsp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qslqfdup.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hlqwepwj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ucwksyky.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hoclteos.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2satvajsp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mawzjtsf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xoemzadm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hyrnuoym.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2loavqcnt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmykwxng.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yrftxmdi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rvtzjkax.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uoagmkvx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2flzovmca.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hgmsqfyf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zqykfobu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypmivrnc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ivdiwmao.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lbjzlaxm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2prmsepzc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zfylwfyb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2knygypsk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2owpjjmah.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zflfbjik.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkryepqj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2raocfvih.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ugijlipj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvaqxzaj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ikwkcvku.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nlskscud.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzthnqwp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mdkebicg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xvknnpem.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2unxiomst.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2glcfjcmo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2flzouboa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ngkpawmd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kekuvlzc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cgggczwc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xadibccv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yvltirtp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2anlboatc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gifqpocg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2paxjwrbj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mqtiyliy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsbusts.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2digihfjv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yvygpbwr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjlzudmh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2enuwezru.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gglwoxiv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ajfecspm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2iflumzzz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2eqmowonz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fonpvsnp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dnoyxgin.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ostipwnz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zqfviyyi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2glpuepgd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jdbwepzx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2efvvqluf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2javtzddq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iibjdvvr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hokybyyn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rfyjekya.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2eiaksfla.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2araicyhq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lmeiyzrd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohjysmhy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2anvnubbb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fvjrwnct.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ntcuwvys.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qopluxtn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crqdrazu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bkkergyr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2lclennxj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mxokgduq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tavcbhna.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oyvkhlut.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zjrkjsmf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2popnpymn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gtvccyla.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2msdbqyfp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oljkoojh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrgczqob.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2glfodxhz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ldghtdsb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bcyiovld.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cicojtnx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ufdnjwoy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ttbjjpde.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lcvtohgb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vtjsonio.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2slvbsiye.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hzjbcikw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2biipliwv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sszranez.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kojhgzqd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mpockisj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rsmmzgtp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mdlwomer.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2blzqspfl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pxeuldbs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2eewpatvc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2isbxhhok.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rczbqbpd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bhgxtjsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvafmzhh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2brshbxua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2feraperd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jzigjzwe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uifnqcgy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wfjwmzmc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zzgizyhu.html


<!-- 参考信息 -->