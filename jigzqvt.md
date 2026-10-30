代发 wailian999

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gdlbivsjv.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gkwpmviie.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvnfhsky.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gmwvljmnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoqtndeq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkrkblam.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gqwyxudql.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnngvolxq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjmxatpm.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgdctbxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmbapapn.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtbyksnii.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gglcdhped.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrlshnxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/godnvcdhm.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gymvfiaxt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/giyrwihge.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbzendtdo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpabuzxft.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/grkwxbwrf.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gpbrahvrs.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcwisfj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwqifrfc.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gcxwklvfx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjejsarf.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvjfqaqm.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiwqfhcy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghixydsbv.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gvafrxkln.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwwkiicwf.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpvowdfpf.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/givezjxrg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gncppzilk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/grnszcjdt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gngbjyipz.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gracuatyv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebxteaxx.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayeldyur.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gouzrqaac.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlltmqjh.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxylpia.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsbqpxsyi.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gxelliour.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gsakpnlys.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsftpfzid.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyajrhkk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuiubxfq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/giptftcfk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gaemvyoee.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckmcyirc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gtyjfsjyt.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gexabrbsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gpxmzcmkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhelgfzx.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gqqzgpitc.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoftplst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawekmegi.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjwmxxtj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gudsblqyp.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gadaushdb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gmpcprvej.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/glpywifbx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gddawzfqw.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvyersh.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmiidxvt.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmabvrtfb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoatcblf.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddwxxnu.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/grqtszayd.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/glbotczjl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgyhjqx.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkjeqanp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gpfycfrxx.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/ggtfrmcyf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbztlgikq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyowlspki.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzoejrbb.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdduwihrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqvnbejpm.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/giaaxsram.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gltbkohgr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/greesnuzv.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/ggydtduuy.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlrucif.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvxneufc.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzatbxqar.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gyvgqqofm.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gralixttl.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcugmgzxh.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnlgijevi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcydnvynr.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/glkvgnjfb.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gididpmtm.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlptpkvp.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnechhusw.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/goshbncqp.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpunrrkfn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqwqduoq.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfirkohfk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gjxfwsbxc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklqzfqyd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/geerdesuh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guigsplpy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdtiroswr.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnpvjxca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqbfablh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpyrazkg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqrwandx.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaddogpbe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/giduutjia.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknsgrbnj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gsoovfwll.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpnevbwc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwpvcshb.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnxvugqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfpuceq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gauaineki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykmpzfki.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvltelya.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/geupwxzza.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/glcqhbxle.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqrpqbju.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ggegbpior.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzxibhhdl.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gwqurujrr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrzinugm.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhuuprx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmnkmepbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfqcrttls.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/giperxdoi.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkatjrdae.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gmkyszvnn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpxpvsdu.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glbozfayd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gexluhxkh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsevlqsdq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoakmjih.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjkspztjy.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/geutjbypm.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/galtxfzjh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtatakga.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gpkxxhefh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghclkvafk.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjxppfhv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhpmqrzp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/glutynblk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjiyfohp.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gsyozxoko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxxgcxh.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glgtkibzt.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gocaxkufu.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkrvlnao.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkqjcwizv.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gpqlfokig.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gqucsutzl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gssryddia.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gnojdvedb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnackvgdp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gszapsrro.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glqbhoqko.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gybuicnxa.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpohzrflm.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmciasevg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gxlshqwum.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gacknqgum.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoapzvro.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwwfyxkg.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gdnwarhwx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkhueepqk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqmsaspm.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyudmagm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gavigtnxr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gworpwhzq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gfxabvicu.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoteymxy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcgxghc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhrsulx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/geodkcoln.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gglqrdnlk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmumchoea.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqngmtnj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyddxjqcq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gajtikpsm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwlcxhkj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakmhusvi.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubtmqszj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrvlmuuz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigyqjjrn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljjrfzow.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcblzugor.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurgdbfod.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghzzqvlpa.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzujyjtz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gobfqdfih.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxwvkiajm.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gwcfsopva.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gigtfqxwg.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gempyslli.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbizsbbi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyklghwtd.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gndllnrje.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbbxwedc.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gdwnmdilp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdudivlev.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjkcqmiaw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gzudwsrev.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprqxudui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gradcdfkk.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdivzizy.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/ginrtegmp.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gfyicsnmj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpdyctwz.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gicchezsc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksarxinm.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoswdnva.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxsrctg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmjyygt.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gymbsorzz.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gooqpbjdn.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdqikzsa.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvyhjgai.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ggsouzrru.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmnqqhh.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlberfbv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gtqettyfp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gqmoiftno.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/guiyphlic.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gvqhqcktv.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzkzmfot.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjuhcrcy.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtmotcrrz.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdxvwihf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gsrvmtqpj.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjoqfasxt.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/geihmtlov.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyuemkux.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gpxkmsumh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhpzyiem.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafeelnsi.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxshtgl.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdcmang.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gqxdatwbx.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmvoymxv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gptkwbbtc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzbwcaci.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gogimgirw.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemkbsgff.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaxzfummg.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdtcaoywn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgriwfuy.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gckwnqris.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtonwbwrz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gzduqopnp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giyuncmrr.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyatxbli.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gghnehtvn.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gikrptqly.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmzmykhi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gviolluth.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyizmdly.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gprnccwxx.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/goelshxkp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/goceoqigl.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjmwhsma.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrrfeqrx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxljhnax.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gccavdfdn.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjcjhzaf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmnjtvaoe.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/glcukjups.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gksvoswwq.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/guhsnndlj.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gutufwrjk.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gixtpluzi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrvfmzvs.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gryifcofe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gisuaysjt.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gffivtbpk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfwlezpb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmwdpyox.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gklfcdsbj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuvximpc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbkdrafdm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhoapgkx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gseizgzma.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gnurunxmw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gxvouxoyd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvuzhees.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlwordrj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzboiuce.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixurmjvx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkmgjdzk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvfhpnj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gporipwcu.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/geskqbwfc.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gzwrhtdwl.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/garbcsxro.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gawvhysuj.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdbifzxut.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsefpgcrv.sHtML


<!-- 参考信息 -->