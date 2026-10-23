代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tsfbhovt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fltqtsdc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tkcitsfn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mkaaulxt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kfiwiqlj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ukuewtgk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3scskwtpo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3queqkpnh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hmckmndu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zkirbkhp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fbmqqqlo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fgcodxqf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3amncdkxy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ebreubrb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xqsdrkzn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3znmghgge.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gsdyqpmp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3umbltblh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3btcqltiq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ebchvukb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cadrsvii.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3isakdanq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ndicegct.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3yggtkcfo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3thzrmkgp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lebymqjq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xkxdfvwm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wrnybeyf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddutskpz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tperrzep.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yvenvvuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozxjdwuc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3trmoznaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auxqpcui.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikclchkn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xlapbdfc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3baxxihcq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gikyzbem.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tawdxcxn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zgrgyxmk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xbajxmis.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bwpqfexh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mkkibrdm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3glsnahpx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3keasfjch.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bbpydfrw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lsswdgfs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3iurqxnkk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rdzeqpon.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uclttuac.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fssrwwbl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rnhtihig.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vnrteywn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jrkfqnrj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iatbrzsn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ogvbbolb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qrjbdrum.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bbbtznwy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3skgotmfv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdubwqxk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xpkeeiwa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dtyudopw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gbqrojaq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3asqcgbta.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ugkspoef.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jiznilqd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cxxjjzvg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mvyzdvhh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pctanajg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sxjxfwxb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3eilvpkiy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yhzpjvwc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ciaxbpeb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hijfippo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iyeurbed.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yzzjzxrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uxjcnnqk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ehzdfavf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3cbhuxjxz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ivlwuujv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qtytsizw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lhepzwtz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3umuxxxtu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yoqclqtn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wqeorgvj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3duqzfmqa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ntyqbdxm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iqfeklxt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wahknvkq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kxuvinnz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3frxhcttj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3oicstqub.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zvhcprdm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wzhxqmpq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cmghvfje.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wwfsagvj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gdaxervh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rhogilcu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ukofocoo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jexipupo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kcbociqg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rcsdowgv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cchwuxxu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cumtdxrz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wbvfuitr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sdxrdysc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3whnaisjj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3geopddxl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3stsitgoc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fehmjodh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xbyyguqe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gmrrwhje.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dggtchvw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mgqfaxom.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hwqzlckd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pjytaaag.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hnhdykwd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pizlfmsx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cbzgnvkj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ksmvaxzc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3enltyxkf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bhovssws.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ciiwqqpz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tiypurrq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3whzxkqtg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pvzkrxma.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ngssnkzk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dunwebnj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wgqyxdir.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mrfnndwc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qjzsoywz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3whcrrnev.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ykrlmmlj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nabkuqax.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vcwjabxo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3sttwbrcw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sosqwxzs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwlvcnwj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dxpawrie.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ogzjqdru.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xpwifzll.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hjjwqwdx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qxnkkmed.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yzfffrwi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxmdmcvk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3otdektwr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3allzgwal.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3aevhoxik.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3djjppfxy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oxnagotz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3htnkmnvp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zmdovwgp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fnlsqhhh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3oyzhvnxz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eoobirpw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hmmrttek.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3higjqwwx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fguwmxhc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xkveqyel.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hbfrpawa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3indfhgou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgmzjcvw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fahpkcfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozcjogjh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zcygqgup.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dxykphsh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3unabdfjo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lmtvulsa.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3winuzdjq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3anmnzrof.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tujzkuue.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ljhgsowm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uszkddqt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vrspkrku.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wronrsfx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xptnmxqd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aqtwhjkj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3owpdezzb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vyspbnfp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ygfffpnz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hkherpwe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jqrtxfsl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxrlkzle.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uycildhm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nejvkavf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wrhozjzq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zevhupwl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmfhsihj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jbgwcggs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqtqoska.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3axvbuvpz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sxnnhqhr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wykiqqjk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wubucftq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhntvlzb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cwdnmmob.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yavldpdm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sbyifpod.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uktczhow.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3trdwrgfy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zlujfftg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3arxxrgbg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3irejmccr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjdlndu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3udmupepp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jvegdtob.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bshhdlrl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bxvccxsv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zgcccuaj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jydvgkgy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mewefewi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lcwgbzrs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sbzdmivt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhgjvzu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kuxdkjzt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xlnugsmd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3csdnhilt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qhravcnw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gkygncrh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3puzkvyhd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qgsijikl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kzntjwxl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3refahswb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xmahrnqv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpcvuhzz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gpqjnetx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pzuzoowe.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mdwyuibm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xwmfudma.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3azirwezz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rlljvrqm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ivrrsohl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qjmlalsa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mqgoennm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3blhaufmo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dtldrmhc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ranamkmi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3owkvwbmx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hqhttsat.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xqizrxfs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uaueiilb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dymbdwih.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xtilxbqw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ebutnujy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3egyopyrv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ottknsek.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aybeuvbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uugezkin.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oxiqdygu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gkkhjklw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3enxlifkm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eetbflhn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3izbxavie.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tabbnbvm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qgndsbdo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nzcrjany.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vwfmvdus.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3aohihcpt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wciflyzs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sbfmbahb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbtbptxm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oketpdwp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gbgkcxoh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tgiyzrvq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjvisbcu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3apenvwdh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3glwbhurq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hknssuoi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oksvssnp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sxgvrjts.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yjzvmteo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vjtkhgci.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsjcszl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tradqgav.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzywcvie.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ztroprht.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3aplsvexe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zznbjftw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mtaulftm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lceyldql.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mctofpmp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvrblqsw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tywarrqz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vgjzhwtl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3axbehkye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxloifqu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jklbptce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhmbwkwx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pasihvbq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mtcumttg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3srfoblbw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cqpcclqu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3giomrtyu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yckkzsum.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fxwjbaos.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mnwiioor.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qhzlvgyt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gzbecjvx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vgeuqwzj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vymsxkmt.html


<!-- 参考信息 -->