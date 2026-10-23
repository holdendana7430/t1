代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mltpzqnd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gtaydnsx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ryckmvuc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yptlddhr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uzqxjkuq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cooqqtdk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vjgftnvx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hshjydmp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fawisjym.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3tilcwjer.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3esihxaun.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqhuwo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zwqgqjep.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnphiffn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3edazvozy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3sctlgwns.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zaewrdkg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vtkrmxmh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3obdyjtln.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lgsgxlyd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3damvmfau.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mhqfysix.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ppuunwnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqujoykh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ytrvxkjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocermsaf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zhjofuiq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dlfeowaj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcftvakp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ojniwlmj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bhxrjxdr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3emlbrlwg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fdeyqqog.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jrnuzxob.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hzrshrjh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qhwstbig.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gbmpbljq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruesxguh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cdxnycit.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3akiuacrs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ltjwesuu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ajgnlpic.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mpsnekdw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qbhqbkpf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eilpikbd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xwyecdjt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nkkphltr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftyhqnnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zggjvkwp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gehwmzku.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vztrudks.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3loqqdogf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vdilipri.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wszshmhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3khqeepbq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mqrpsghu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jdtubjcd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3suaiphgb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3eioqfqbc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3wgkkfgfa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ufbupxjj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rhdfftcx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ryguzixb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ycejgaor.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nmlwdaye.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sagjgxsg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xvoarqdz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3weugzqls.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zprgmrbn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sxijlyei.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jtqfnugg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tamjvsoj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bmdnqdnh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ynxitddu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pulguqdj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3juewllpw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3euwtvrln.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3teauphkj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jznylexr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ribwfegh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ekbfodoi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vbkxcxor.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfokcy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zdkbefpy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mjsjvhpj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibizhuqi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zmwnkhob.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3eeitbhua.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3sacxdkja.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zwinypuu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ymenyhry.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dnjbujok.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tkozeuzs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3eduxklaj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwvzgcjf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rrbxvdck.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3eczxqzzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wntnpjtl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hkqbildz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bmuvvgls.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cmukzidg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eqonwfik.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ilwfykss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqidelop.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aafkmytl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3abogxlvu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mugjxens.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vvmmhtap.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fmuqszgm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3csadjfea.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bryfnnqv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vaqovoxn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3noornhfs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hooiauvr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksomhsus.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ygenrusr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dljncemn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eexedoiq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kejdliyd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wwfygqbt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3evneaovb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ofgslhti.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3neizicqc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3krmlcfkx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3evmenobp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zwcqywnj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzwfgqcg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jsttpkdj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sdkeaupn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ubjwulgp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ykxvpdha.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tiskvuin.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dozsoein.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hzcuamgu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3oqnkhzlw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ccotuzcr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3alljumio.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bmoudefm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wozrmexs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3oklvrupz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fqeshltx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zwgcdvqq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gkfcovjz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hkwfxwij.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3heybfolq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pergvwca.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mzeotupj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dqltjhir.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3klffxndk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kyocojue.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3eupxsizx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3twlqjkim.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dulgyyrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eajgpdui.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lzrfgbww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyxgpvzx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cvqwukzl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3raedhkge.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fjzxkwwv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hgdmzwbl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bxoxyxyh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wrsqrrif.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mvandwig.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pvcrbehd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ldcschpa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fbtbihnj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sojbkgck.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dlwifxdt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3igvrgowv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hexevmqs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jfgkuskd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gbnicfqx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3psysiodd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ocxdudxm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lsdszgzh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qbbduutl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xqajbzjd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hkageljv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3sxhjhiwk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jejkzlnx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tznwbjvt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3loxflzhf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vmzhqtad.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3klvidivx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3flofhiiu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3eizhtjje.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3radiyizz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3palsmrmm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vwdmesty.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3reipwvbm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3amixwlzw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qibrssxj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3inxbfudj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mbxvvmcm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gbknqwrs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqksrhxb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rejqgqus.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zzyqaxtg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3opjpxvxu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gojvzxcc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcrwatwg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xjwwijil.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3seaphzkv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3togjyrbw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3uicjyoon.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ijmirlft.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kkcttrlp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jfkiomhe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zspwhteo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rbkrrafn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uqyocryg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mkcjoied.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pbwpesqw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxmzzem.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dvtmjuem.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hufxvswf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tajzivqj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kdebabph.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahsakner.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3urbhulzk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tmjhuwey.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3negrzsgb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pzjcnfns.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mqaddzla.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zwwjbcil.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iekleywx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tmiabgwi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rvhjgzfq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3saazpwef.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vommitdc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vjnyhkxl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3izoftmyd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yzhqatyj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lswtexdv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jybgehah.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cpdbjadj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3csilyhrd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yrkjqkwq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmqioqyz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3arywteob.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cxairvcl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tgrgwspj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sqfkgalf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmsvzezy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wgsqdrmg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3deoilkqn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jbvgutpf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shzltbhp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bekgucny.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bsrizhta.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukawtaku.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kfkekbbd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgkqmomn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stztqair.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3srnacznp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xefpokbo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhecmprk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yndkspkh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3piptepld.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iisaerxj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3epxzwank.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iptastej.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cyuysqst.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rxjztern.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3econnmma.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qnutsjge.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ljrhttii.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gfsbfeon.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bcaitjmm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3raztdigq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iwciidte.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ixbzsmox.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kmbavnnq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3umlnzrre.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pxseeevd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qdbrvsjw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rtzyswmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqgefqyb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pidhmnxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgrzogxk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tpmcddsh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lnnplehm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3klteboyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwcbttbl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3eswuhgbw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vvsswthz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yxzufmrz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3udkbukoq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nwblhxpl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ebssiwdp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xpcgkiny.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3oenwsxhz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3piijriae.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nigpfhxj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pympqoer.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wizvgtur.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kxspbrgk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cdybqeml.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ffobaeus.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dzvevuqi.html


<!-- 参考信息 -->