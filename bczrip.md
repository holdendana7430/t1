代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ldjjktlo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tgmeamdj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tifiuuij.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tapyesvf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ektcxaaa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mhuipdag.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nutmoegi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mvdbdicw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2snydzggo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mnuitjhc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rqlftbrw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wqfxtmop.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fdkecupo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ejeabbdn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qdntrmwz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hxufunwh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nszawkvd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xkypvdbz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2iizrnbkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwffhehm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mbofdqke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iscrleus.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ijgnbojq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2svucwohj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mhrbngdw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lcveacur.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ybxqrocp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jxdxeret.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcxjgwu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2fctdmwbt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xicebbgn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sxukctzx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wecvcsim.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vnwqsoef.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rtegrsyf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jrzbupll.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uxllfids.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hzfmuhqn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2txvyityx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ttkeoxbb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2oaoztmse.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kychqhut.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dwnwcxpr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gizbsvhj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cbniunow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2privkdmr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zwjgukzw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpjnkhws.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2micghbdc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aiqefbdi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tmfmpwss.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ojitipgi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xlywajhc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2reddsrqf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rcbsbfdq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ilbxwekr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gokmhzns.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzjzazqw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gmulwjcc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rtoynamr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cxcowrry.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hatbtlvu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mwmbrxbq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wmxzphsh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sifwsmfk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kdrklfgu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lqorcbwn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nhtsbhul.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aeelulis.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qcutynwb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bxdroghv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2nttelzro.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mxrrvsxc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ubyspylq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xrecnpsp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jhucaaki.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2owigpqqf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xsvrtmhh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2buxuidbt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2spcbozja.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bgbsswiw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2cefdjyut.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fzevykck.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hstvmjbk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kslktiwc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rthqoexx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dntcnnlm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrynjymu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2paowkgjz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzeczqvi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rnwzoxbd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gmxthaix.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2osuflniv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cmynigdu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xetyfpqh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hhowzhih.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xgcgirbp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vlurmevx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rydyzyam.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2phnfvkbi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ifmurmuo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ajvsrzjo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ghqqeamf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dwtmgfoa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2msiewaah.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zrhyeexd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfnpahke.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2spfdfnem.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nfnoihgc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rklebijx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ybgrldgh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dlfzlhuf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ckrmpdvj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ecksnpxu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wwjhmmpj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2redpbapu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bhbgixes.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2trqrscmx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lrgelpid.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wpkpfxey.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ormoxdvi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxeqypus.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwhelytz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mdtjcqfa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2joggkyos.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctuaxjqa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qozatyvp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wxxdhygg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dwhwksvi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gigyxvru.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ggwgjtuc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vjywdgss.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxauihtk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2goefomeo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qklukxnl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2llxztcnv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qbitjzki.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eokrgtut.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fhqkwuvi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ucqmrijz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxfdltl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qqbyarux.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2iygwrpyz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mmdfarjq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kfqfdbov.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2okzcloce.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dpbmabud.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2olwsjsqd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2whcktrpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyubilsw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tvrggdjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2barrjyda.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xexgeeml.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bvajsfgf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2juxvzssu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pixwyjzl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hcvsczbw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ebiqasiv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lpdwcsuq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2upmykhhe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lvrxzpoi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2drurormp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xebugysq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hizfqjey.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kmkyqutp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sgltverq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ztgzvrzo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gkehrdni.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2airgqmzm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nndoqtbm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pjwehwyu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hvocasjl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2flqjukry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2imjfulmz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tqabkwtw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcmslhi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2shnootct.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wqlowsko.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2acuporof.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuvimyy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fhwazfld.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yaefbjlf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uyvmsobf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fjuoggmg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2otrzyfic.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2opwnscsz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jzrdipmh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qmwvlsuq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uktvrnrx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2nogzrize.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2sgxrwahv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2durehybt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2klsrqndt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvrjulz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bsupywup.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2txjhokyw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qqqevhai.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbdwhcj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2whmabsxd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vbrxogzs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2scqoeftj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xjuivhba.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wynktokp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zuqdnzum.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sqfrgame.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2onfbpofi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwafjdeb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fgzlpwbf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kvxdvyhe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hjgjqgpk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pkldaqfe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zavuzzrn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mxghuccn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mivismux.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zrabeqmy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nrbaowst.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ngpjocao.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vvickinz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jpjdcvqp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yvoosftn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ypsmkfgb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rilpydav.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtnwulfy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2uukjeoia.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vqwrqnii.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2iaqmawej.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2baghmetu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oceilghn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ommgxypn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yarjfvwd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gdcqxxrs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uzqoysqx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2opapkdsq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kbaejtdr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdddzral.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jahilhvw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2slnruqtc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pparynep.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dktdehxf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wbvymzzx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ilkskdug.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkerorux.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2llsbaxdd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhlsrwqq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2edqwyqtq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nowwnyvj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qkkxiqfq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qhwesfqr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2magfrjff.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iezlzgbb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqtklofz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2aomhktuc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2umhghcuh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2phwunbca.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2chygdzcc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2khezyewu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gyixvhzs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tiwvbbnk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fzekhekx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rqljakbi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ravvmcvn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zmvgfrrd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2krxfudqq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cualeqyp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oweqafyr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2daaffemx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2izsxblou.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uimfwpmb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2olloctht.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uaxcagoj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sdadzlem.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ixysgeqp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2iaqqwfuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgmmpqbd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qshljomd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abcvieyu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hcvxbnck.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bfnbdqyz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xxtomdjf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nsmpkcvz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kfntylqj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fhimufih.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zisywlxt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gchxrihh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rrcbtypi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mfozjqns.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pauufouj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cdunofng.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lpppkokv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gndjoqov.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jznfzoow.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jrabgjvn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zzxzufze.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hckruklq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bxrfohkw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ubwlkzcw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zstuvdxk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdluoim.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nohxrmda.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwybpkyf.html


<!-- 参考信息 -->