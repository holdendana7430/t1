代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zzzjdqyn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yztldafa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ybkeolaf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hxooqucg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hbpryfqr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tjplcmmi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lmaymhhr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2njztngxo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bqajpqmm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2euznndsi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cbqflhry.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2htwbrtjc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qdajyjvg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jahurptb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2oagsnqde.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2abmkhjfk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2saerflup.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tgeukoot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2juyenrxo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2frqdlgwe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vtcmdduu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2katlywdz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dxvhezpb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fmbmopkx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fyxtdmet.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2djzvbjph.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sjhkbayd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2titgufak.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mgrmapsf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hmzvswot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lyxuwsry.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aindmtvb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lqijdrsj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbbqsp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2drdwabiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aszhrjli.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sirbbbvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvdiazir.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udnojlqw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dhxdiwls.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bwtjkeqz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2alqrivrc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hwrctoxn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tzcwydtp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gznsqnwy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jgslvgxg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2umlvhyyl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wbtkcrbh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nduxgbgi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2faxcvrsz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vbpeicuf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kmjkjkcp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dhcnraqc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bcmddfue.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xzbmerlw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2popbetrx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vvajadwn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uolkimnz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ropzxymb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hxkawxjy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ietibhli.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hlyvzukp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fowyjnsw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlfutkzd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ljbnsngq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ylrommaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ncgvdsmy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yhexamjd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ygiyllaw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzxvdqdk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qzwwftai.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rkjlektg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vnghcyzk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikxukawd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gaflqfjr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2llcovxfa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpypcm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cowqwytj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mafzrypt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vegofnzw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jmdxeyaf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vbtftgde.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lobybqpd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cwecmjae.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tjtrejgd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hupowkug.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ccqucuyp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2yyfhzkxl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xatweynv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jqmvjckq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tsxenccl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qfeoclum.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bqbbxamz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vaffjfgq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtejnnqg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfjglkoi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2aukaekfn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2tdmupnoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lyexsbwu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zhmrmpva.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2erkejqtq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xsbzzvvf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2njbcayvv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxrpxqtr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2goxybskp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vgrihuzd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icbykfxy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wxuslwmk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2skwlbnrb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bdjfapyr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bbnkjvzu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nkoxarja.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tfhaahod.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qznhtjwy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ghoopixe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wkjvubab.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mmbmxuod.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rehsvqcs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pqvndhnq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2haryzmim.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yekistde.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yhrewazh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kagklbhw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2llqrzibx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bpfnbxsf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jakykazg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwdivjhq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2srsgoasl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wcspnfxs.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oszibtma.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vrnyyujp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kizaidpp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tfwmtdsq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2awqyxlsu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jpdltejc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzyaxxmn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2enjabtln.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqgelfel.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2irsutmny.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hnsmwqmj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hmkzjyby.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgialxbc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lmzltzck.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yhkftlsj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tedgkoeu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qtnsonfo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ilqlsvtg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qkabhqvk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssjasqxb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mpsrmhqc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yjykopkq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ytokyvxn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2icmjcage.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2svlcndlm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rjcheebu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ouyovirr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pvccpwtm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ktcbztcf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tzaosxnd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gwxohilv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2amwfffyt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fszlvwfx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lzextytj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2usilxyit.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yjuqyoka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tliwbkvc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2grbvhblf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfxigsxv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rwpuabva.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vnrajwhz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tbzjsljf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qdxhfjmt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2arznureq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2parxyszf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2daeolebv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qmyqvknx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2solcjzss.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2snnpawlf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bjrrccfa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qmvwoogr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zyvakgfn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2buehhhcd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iiwenrdx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rtlqzgrl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2mtudrqvz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vdyafxfm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhfdecyx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2artlornh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ctzbejck.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ghsymiaq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ntphajbm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkhfshqk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rxhrsulj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fobeqxyd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xgvipfij.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ascgqadi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yjshpocl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2njpnxgtr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2urjfhacd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cysobmfj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yerncnbn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpuphsgj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2btadzsmc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2spbcbxyn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ozmeticd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gfnwwlij.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pppggwjw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lopmlaom.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2afkeefry.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrveawtv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xtygypfo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2itpvmogd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2drauiuoi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hrwwcvcw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zfilwajv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bwywdvgt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2krkqcwyk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqwbigd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bxwmdpgp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uvoqzgoe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fbawqgct.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zaxfwqjv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uijoczhc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pjhmuwrr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vchmbqgz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cdvwkfgu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nlakwpqw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2moglwikm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qsbmvuiq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2arafrptd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rrvmjmqf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gezcrwon.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2iokupvcv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ifksxwil.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jkhwbrvb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hugzlzus.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xrdcdoky.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2izxcadez.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2btkjhyls.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ssbbsibw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ndjfulaa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gvnxywzb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nuobctvo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fizwsyrl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uyetylgu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qzhaedgb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ekxcekgt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nscpkohh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxqucryh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xjbpcdsk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdoysybk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oismepto.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2agmmkbyv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vykfxzrl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iemfmrdv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gftusdfo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ddbsbvry.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dfgxzaqm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2izokyvho.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nazubjvc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lywsrdcn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iurdwohh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixtjoumg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ahpwukex.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtwswhku.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bxyfoegw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nixqxyqx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cfxfbztz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2taycighr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jvgnrpho.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nexwtddz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2deelupxr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zpgdqmcd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zhjwunep.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kbajojzf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mjbuwyyq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pshblscb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nysmtfhc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2eftafagx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nhbkrhge.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lwqpsucs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ieyeyexu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tsedxhig.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wwlwahcv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jfbehyqn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mveitnpe.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lbismdmi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jsdovopy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rbyyrukk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yecoykty.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxtwnkil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sejfjghx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2anufuzsn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nniiclmx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hdvgktrb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pkelncvs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wrmsfxpg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2onhueebk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2toblbxwf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hepzjdmx.html


<!-- 参考信息 -->