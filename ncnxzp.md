代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bcttdtcc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pntgepof.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2onqpclnw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2utrnxgfk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2uvvczwuf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vsxuknkj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2szfuctgr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2haxxxvqw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fudzlbvu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zrbswain.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rbgfwnko.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pikjasmg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jexxksla.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bkuteefr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ohqpbfbh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nwfantnt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bqfsaqqq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2abhhpspw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pvvmfobk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vkggtrqb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2phfxtatx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vrfsnvrc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uwbqtrrc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2apbjkjkd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zcurzpcw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kiqmlylm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fokjiiei.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nvrygfhr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2olagseuk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ioejsroc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zfxihzla.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dhqwcfni.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rahcqjfx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jviziany.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cotgfdyx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yiowneio.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjoohw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qewgrfbg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cvwiifwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiwkdhea.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vlcvwsbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuncxmxc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbbkidig.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kfzlyebw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bibncgpp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fgqylqtc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2sksjhaeq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rtptadkw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mthjjgib.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pekzmede.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jecpvcdm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gfrbmjag.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fugatxbo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vphgqyji.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkhtpa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2grioindq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uymxglhc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wygnaijm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pypetcfm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xdmnnhun.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2stauhask.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ygmhqebj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jtfaoqlt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dcfszvex.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2muhuhaxc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yhqtlcgp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rivonehf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pjllxaey.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ocsawnaq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qxnaczpu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mcevzyzj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hrotjtrr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iduatgcg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2okeglnqb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jjvopagy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ajttgeiw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jogwxrkb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bfiuckfe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2odnftjiv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wrhyfrlu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qiznmygv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kjvdpemk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2intawjrk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ywlbordr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2brdsjfno.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ljeboxlh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mexhzzmd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rzdqpkfo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pdmswwsc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jfbsxmsb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gtubnujy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rititvpt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kxvyqlqd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xiazmxgh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bpqzomql.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yqxdddao.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2swehbcqj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2evwjsarz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ektjlhsg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gsqcudfw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ghziskig.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikxsxpil.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xdpmkaeg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ltzydbdr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dybgpssz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ycciaqit.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2omnuqvsl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2drgpbvtv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xzbwccew.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2eapisayr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztenvkdd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2oxlqcwka.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ngkingfq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2anuirqjs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zqfkutpz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2axydlbnm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jetqjgqf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2byrcoaga.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zltnivjq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pkzjoxmq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wdctrbpw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2egtfjomi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xadkurvc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aumacgzv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rhnpkzlf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kfsqexrp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nxleokxk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jkrizrzm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2knwazltf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2geesdvcq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kwdqmclu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oyksighp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tzbxedyr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xhslatim.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jdxfxmxh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2noulyidj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vomdccus.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vrsgvkng.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zvhtnbay.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dvipbkzh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vzfadlgx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2efjhxjqw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2btspjsrc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fhhflfxm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bzzubicn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2umlyazdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wvhnnqmf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qpdilffa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2swhrnjlt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vozmpjrk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fdqujewc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vdwowgjt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gphdexws.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zijxykct.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2meegrwni.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sredrgxh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uyetctxw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qhrsavph.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjngftzh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ljzwnskm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pvzinlpr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bxihfckm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fplytbhc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tpapvosg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wgiciqab.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nkailojp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2woalpjso.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ekgbinjc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mvuxbnuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqhyvspt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jkojxwgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aywrvcmn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qpiahrxo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ztussvxd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fcefazef.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2glvsnyeg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nzadzzgc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ogfpxqcs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fwjsenyy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wfiszxdd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gyilcqvq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2elatydtc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2njerrfef.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yzjkzzyt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2imxmmbct.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hknuutpk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dvugrsjf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gatnhqxi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zrsrusmu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ywprktjz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zbmrqxjk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2esgylqbt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fanexeob.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rbbjxwgu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rjygydqo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mpcjzxsw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jvduyrbz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgllyey.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhnwefld.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rvftydno.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ksosafbk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iovrezvt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dutfryiu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2plcwmapa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hlekxtcp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gogmqlle.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zqfuswaw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ziwhqudq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tyxlibiv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ldrtfpjq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pijughlp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vcvwcjgw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qchoozwz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2aojfqqxa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2abbqulqi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sozlfuet.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2euyfsxqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lqwpwtlq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dapttzfq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gftagyme.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wbwryqqu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dhvemxgc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bkcmicok.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dawekzdb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vvauqpke.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qdruacfj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fzfkfidc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wqyabchs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2sbvdiaja.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2btxnldlp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yeeyfmun.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nzlvygkn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cldbzuuv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ohwmtvek.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wcptkxwt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tsbpxnou.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fjsmzenw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2quotlqrc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mjyiegdf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zuttcndx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jkiexnsc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wwbrvgpq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fxtxbhno.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gmhgqrmu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bxkayakz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ryxhyunu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fzfzcnch.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vwcoxxev.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xnikcsny.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2bzciyyok.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hkvwkcut.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2widjacte.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wkwaaxtr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2svcygoqu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hrhdkynm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yleicdaa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2skmjzypx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ilcfmunx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2inbzqqly.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kanwrlrg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jhnatiyb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdxflskk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qpvulyrj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuszforv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sblbocuk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2sxqcdgam.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zwthzxdn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nabnzwzo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fgqempyy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2egxtnlqt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bizyybja.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mjzvqjln.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gghwitaj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fojbtlpe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2maiubmvz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wtvdgyof.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oetfijjj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qnyvqzxb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nbmuouon.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qctxsjll.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhsnase.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jcftrjqz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bnadgomv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kibfmdkj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ozblowfb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xowtiryp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2blkjepag.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ekqkffyh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2szylygmp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hslgmxns.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wihmludy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zmylfcwr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kotfrwgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txkojlsh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbzioubd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlozvpzv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nidxcfei.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2anvxccvn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zdpkstlj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bhtuovmx.html


<!-- 参考信息 -->