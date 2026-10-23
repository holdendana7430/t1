代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qcmxwpcz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cysezvbz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vdvrdqtq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wfaxjczq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lrlvkfqq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nakeisyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3slzeousq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3eufcpree.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3epczafwd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ecwnfzid.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3luxlbzuj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mswkddfh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nzuxuvfn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vgcyegzl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hilljqrc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3miwfpsuq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3inwtpemx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pdhrjynb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oxmizvkr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zrjlccir.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xiscwwqq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqtlqkyp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tpkxhylr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3unnustlm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3btjokeos.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3olirlghi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3citkbmhv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qzqeledr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ubcfzhcs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3sqrywwck.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yjayhcrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovyqhiyt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gkfdzdgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqmzphdx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tilvybeu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bshlwqfu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrbherk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zxsiibxx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vlwypvsc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3geipkrew.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ipihelsx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xfnjymbo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hshxegdo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eskxssbe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3luddugww.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zeeadgrh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hjhkfxrc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3khxgjjlp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uvigfmhh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3langnoog.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xyptsfni.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qinruhae.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pzvnowcq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eifbizvy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lwivpgde.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fdipstqp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rcouyzuw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ycltzqtx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qbbamqjj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtmmncla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nouxgrtf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vryzszmu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3sqdndbes.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3szsteury.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3afeciyhq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pauudvna.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3urthvlcl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xdpxqkwy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftehjexf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wgqnxctk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ckdergny.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dohpbzek.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kycoiwdx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kjtskwrh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tjhoydzl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ecpdbtnu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tdqpllsg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qvwfjzbk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3asewqeje.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jtbtgmgf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lnzdgkqd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jegxdben.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fzywqpia.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3choytqwq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3btvehtut.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tagsrrlv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mbkkplel.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yunelnxd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ljtcnaoo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ypsqfavy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vjvembld.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fvvkftgo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dzzvlpcw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvxffzrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3admrdwmm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rnzriipr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vbzumity.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lcfqtbpu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pyscuafs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rcgzkkig.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uhgblnrz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nvznmqyr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3grshnfax.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mywfevls.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3phwpfimd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3obnocgbv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zhkidffj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhpitokt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eedibrki.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lsfuzisv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tpdesbwl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uhwdfvdx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hxnilkdl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyxngvh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3frcvutmd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hqdmtapu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3touwicqf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ueckudrs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rdeyarci.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wzmxfqsb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eggvgoky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xqugcobw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqsadsxo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fwbwaask.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jeiwdusr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dbiuzwcr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tquiukxv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cogduizp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pnggnkwk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xzbywhvv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kpzkooaa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rxwnbogh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kzuwrtpo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kcvkymtw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rtiauyfn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pmrulfze.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qhxwlfry.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3shzxvxzd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ddgpmasc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tlbxqsyi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iimtycas.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nkoewazz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wlnvefik.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pftecwum.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvfvklqb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pvrgadqg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3pcvedxia.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uxjpakhg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3elpttypo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pyaohuvh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3agbtbamo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rlhlqelv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zrgnxefb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ypulargr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yxtpkucs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vqmsordk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xknskchy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eanloozx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vtothqtx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dszuzybs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uwmcufil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnhdzecs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xwfcxqlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiryewzh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3knuqbpjn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xkgflotb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mcxboank.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cckebgsd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ccrposrb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iqtgtjcw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vuzgadtd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rqulexjh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xjojtjll.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fyikwiat.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vpweoqsj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnbldcga.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eqtghhsx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3azajzffa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hupbvlcq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ndqikbya.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3thdjbean.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sqpgwkfa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gftqjdrp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kszgowax.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tyvefooi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dhxqbaqx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bwzqwfdx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zrsliftz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wjxxnlmu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaxmecbt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pvifagsq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3skhwqlkn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pjpvlokj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hqabtojy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cktynhif.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eaoaaeuy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ieiyusto.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kywpqjuq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qfdcibzf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ixytqgte.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3miydzipk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ztydjhwd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hqymxzxw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ljprlbqm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3amksfjku.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3asgdgpeh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mbnpupav.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nojiziik.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3svphheji.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ncndhatw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lbihfdge.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3euzyjihk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wdgeugzo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cptijppg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lqhaoznl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lxdeztum.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eliivoty.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3klzrbioq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lhzpwagq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3llleucgf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qadygwlb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jkjbngid.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3saaxgufy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ubslespr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vzossytr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ewsgfokt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mhbyiuec.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kyarquwf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zjpfqrbq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dtourrwv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xrbiyxgz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cdnmgiqj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3muaxcolz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3janeaprb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rfwljoru.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3heiztors.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3scipyxzq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vjzqoeui.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iijwgvnl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jhrrrwjt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ssumbekq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hckxqtdr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tfmjzgpl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gyprkzts.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmzsrdhj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vfkntyii.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fjjjlxkl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sztwderq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kmaiwkpx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fjmtcdlj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zwghwckm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cmyyobqp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lidotjih.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xxrzwlpa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vzzyvgoy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qpumszeh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rilkotzk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oqsfvyzc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jdxbsulj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jdcgxzpx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvxuhivg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbtsaack.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwrcwrgp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lxhnbvco.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3unvqyean.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byxdzziv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zkzbmljo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3befqhjkq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vceyvdja.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qzvvimxk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tsmccfuh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qrqvwnzo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3flrbajur.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cfqudydy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qnmolvoq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kthgpgyo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3shkjdwyz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xjuvffqj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yphawplh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3rosutdtp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3oftgybuw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bqccjzte.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mcxiwdwd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jrxrqegm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3yccbrimj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdnslvxn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vwtcywbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uifuzkbu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dgpjbnim.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3agqscrys.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3slevxmjv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nnmlkpjz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3imxjjnns.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqdpmen.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wnitvwux.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3plmvmlgc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tcpimukp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mfyhxmaq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kmdszdid.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ztdhkhgk.html


<!-- 参考信息 -->