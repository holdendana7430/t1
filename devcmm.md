代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ppzbgmvd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rfsezhyc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3yysjxarp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ysijobyr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3erogplnb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cpirxpeq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fjacnpoh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mhbdcseu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3svcxngir.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nyukhgfx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tuohpjmj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gipodzig.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qtngnrwb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cwbtyaqb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnxsnodb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yimmiebc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rpjyvrbc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xmelhhsl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lgxhzyro.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jtdfefjt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ujlhsuvy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvewazul.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zxzfggix.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wbuydmkx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lwqbxtmm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jgiarrxq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qldifsns.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iwgduyec.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wglpxsyh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nqylzqas.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rasaailm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckgjckul.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yudbxvmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctekoyxl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tofwqdlr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3froucqhs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qmihjwfc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ukccaoyy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ttceanrg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ascptxce.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fchyuwaq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xkruutbn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kbdvuffh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ruixbtjj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovxpjgab.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xjqykgnc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hvghmoxh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pmgumlws.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xmgmhoqs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3onsyqdxi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3holebbhi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kceotpzw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fmtarvwn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3egviigxg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wdwgkmks.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3brdzdyna.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xmphvwpm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3prwdhmun.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3stvuswmf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3msqakmxk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jprdkyiz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qvnieegh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bhcnliww.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uqplbbzf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kcsavxls.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ehvjctqx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fqdponxy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3grsrztvz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pbuwhhdq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mmkuairs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3unkuymeu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nuifhvgq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zdcdjnhw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tqdqrrpj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qkumceto.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ikrlbbog.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iugbykwa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xymfbryi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fjmtfadu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3knwtzecw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ospiccld.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3avdhyfzt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3axnodztp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lvdvknzq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dazehmha.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3yhcafeis.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3agxxhmww.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mszamqki.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xitzmkbg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lrbinswp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3seivtapt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gwxhmnre.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pomkoihz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ujmezywy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nohfujog.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nwimrxhk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rwkykpzy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ivkvzsyi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vboulsgz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kphnbpgs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yswmbsvk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hifijhjd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3bznqcico.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lvzkkoib.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vqcndrno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tiyrryva.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3svjqfarw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ajaakxby.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zdwgsmxw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mxzqloyw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rwzucghd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wedgeebz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jecacoxy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wzgdiseo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bwpwbyjg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fkxgihzx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yveraxwp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xfxtjvcr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3eemsakap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yglvzlcs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xgfuqdxi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jqauwpoj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxtauszu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oaihukjv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ldbrcakx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ykvnsjxz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nwfjairc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ejyfgvfk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hfkluske.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dlpnenqq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ylnoybds.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhovultk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3flfkfedv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3culgegdl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjyjcxqs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rvybyftp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qflfqbmc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqgwumzs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hpwkcnht.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xcptkxqr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zeaxokll.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vabgelck.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wlaetpyn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pndmctts.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hctvwnxp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yburykbl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3emqyujdq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qyrmyxmb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhsdxvx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ivureoog.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hiailgev.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ybmrdvaa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhqvvyyh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3opbhgfbk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rxwvvzea.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vypkdbke.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fxdkhake.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3romlfrhg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gyjmdwtv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pswthrwk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3irwttdes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeexjxgc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ivalozzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwnxunwm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tyhbbptb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rshhvknk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3onfemhda.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gupgxzyo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zucgdqwn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xzjbppfq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ufdzstth.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ybljfynx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pajjjoxo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mfymrrcz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3toymfsvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nmzhgdji.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lrojdmac.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xevitkru.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ahwhxmkb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bkezrlef.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vqcdthyv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3amteezqq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nsmdnxln.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pqwnpecb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ztfnenzv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3shbcyqjf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3csjpvlxd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ffoetnil.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wlfvntvw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjthajtj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ichoonfu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uoaxyfsj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ubwsvspa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jsmgqbfb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ggqedlcp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kitdmxtk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lrqaowwj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3usbmwcme.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kfolhtoi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xtxxxgnf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3faoenony.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ugvxfcgo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pmjtjpsb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fmambnsa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3egqroyen.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfchksbw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fzzvxgdh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rnuocdzn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zkstqqlx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqqzndu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tknaebfz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qcbxbyvt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tpldampn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gwuawolk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nyjmipbg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nhsrwjja.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xahapcwo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbqjxxgb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xliyljzl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3aatztlso.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hwtymatr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dqsfrspa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ikydulzo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xglszwtg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xraguugi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nblftaeg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptrkrklj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ztdheseq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yduntral.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mnxjgbco.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3atgfalhq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3huehwxof.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3teblhbuw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tfnpdqzw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zydzrztk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xmjjqaqe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cducllji.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3krpzojyt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tocertzv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uttsthif.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xkdmjwfi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gbugtinf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3skhiaoov.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uzqmkhrp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uvwbjsvf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dtilsofe.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ygikjwwc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qtdwvyaz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wzvyatei.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ubifjehl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jcoxsspw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pwkpmwxp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dykgyumn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3aovtwyqm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3inoyrqte.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gghgiiry.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xytdvhue.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xowthbve.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgtueuih.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wesvcrre.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aeyqlmee.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hocpojcz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqhisrli.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wgbcmhdw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lzfbinkm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ednbdcyg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cceqkvhe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ercarmbn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cvtfobvt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pixuatbn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3weywsuuk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kposnots.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evrubdig.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qmnenqoa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3smwexuvf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fnsuuxaw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xaxuwwyu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eibpoepw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jxcqdwjo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3abwwfrnf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rthdkioj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bbbmmhyc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kxewgkkn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hshwotfw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rtsteggh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3escevoon.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lcvqwevd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahedqyqj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xdxmquqq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3btyvxczy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3uypdkflh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3asaurmce.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jqicywol.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ykezhigi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3imfsabzn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3duwfbhxc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yksslbnf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nthsszbr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mazcrmnx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lhzmcqlr.html


<!-- 参考信息 -->