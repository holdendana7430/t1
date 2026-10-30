代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpcikjcs.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/grrcvqedg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwoauyp.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gfmlvdfqi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gkinhrkfl.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzmfpnep.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqhcmncyw.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcqlgefj.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gbbhcbltv.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/ghplznlin.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuqkarea.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwicusacp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/grozhagjc.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyokqzzu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxevxem.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwjbrtla.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gecivzlrs.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gabuaibgg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqqonobt.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqpebcmy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyxuweeb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoraqnlh.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gsddmoyaf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcuzvrfm.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gphpxfcqo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfewruuri.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqdzermyd.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggipozogb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmuxpyisy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwiegitn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/glilhckjx.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gpsrkekvj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gimtiugaj.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gitttjkrf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjkhaobd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbufdlhk.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvrfnntnv.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfumltqc.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gpujmcdhu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gucmagxnd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmxbnjuy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gforqladk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/glewpmgly.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmspcdlw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/geaynrfya.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gjaccuiyy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibmfkpdh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaoldzfj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gscsjjzdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gbottzroh.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxksrstw.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcltejlb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gczmtisqi.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcyqjzkj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gaycltpsk.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfnmgxmw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/ggssilyxo.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktbrsdol.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gyywpejgr.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gsdhzjndi.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzjllei.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnphdhibb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmhducllh.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzplapxhc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgzhbvug.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/goshkgndm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvjuldgl.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsuflncn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgkcrist.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gvdommcih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/ghabhdbqp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/goyypsdii.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gkudnfple.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkkvbrdz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvajwcvtj.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gcfyghswo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmzwpzmn.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsbbhvdsk.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gutwntwlp.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gsvihkljt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyhdqkrr.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gznwlofhz.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpiogxgto.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyubristg.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/geucdrruu.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gedgdwtum.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gzrmykugl.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvndxzmz.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbmvqnlew.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gllpqbvig.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/goqxwojql.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtsqytgg.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gyhaabcjr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzthumxy.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxfwshiv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzhxlhg.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gukmqzxcs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grbxyjyfq.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gqzagxzst.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejibqwrr.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/grwxdenio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gndsltegs.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gjujzjobh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpwtpuhs.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtteuqww.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/guybbzply.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvgwaajxt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffqiiobl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaultbifk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guittvtix.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/guvfjlnfi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gogphaiqr.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnqcmkqfi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcumetzdi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypavfmyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gvyiwinot.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gmiwotzbh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvjlkhcj.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ghdqxhfef.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guusqurkn.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydbiarwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghgmtqntf.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/ghpbwcryz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzbnxsto.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybjvurtw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpzzfotss.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfavebwju.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdwexurq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaptrmuz.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwnrncvfh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvwhhjcd.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ggolkwukg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrhblely.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibjfsvrj.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/grgstecvc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/guvjhaask.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryldzygu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/griazskmr.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsliwkjml.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gleafefuw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjlhxksqn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyvegwnx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyyzdcia.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrofehjp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpsomujaq.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtglkudwz.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grpbyjgxl.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gjxyjocjd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqlostaf.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrsvltdx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlmbsgzy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtyejvw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gnthbxexu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goungcxid.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gotwovdxs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gryqplgfc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfufindb.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbuixitkv.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbpykmsw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ghstcngji.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjumeopxh.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grevompjh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/godtpanrm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahetersn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grfdzjhlb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gysjvjzvq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gsoyvjsdf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcyaadrb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gepmzwghs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkndmkvy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/grjganjug.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshuxxnlv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gswqlkjif.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzavkasqe.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gypyzfjja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gffdwfmlc.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/govuuvihy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdqwaejo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgqumztx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnzrthtj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gudnnfdyo.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaehcprl.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuirolxb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgmrwxsj.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gaomukmrw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/guspdvvjk.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnillbno.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glmqzfcrv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjjplrvh.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuovoikn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktnnunpl.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/galbrpftu.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvelswook.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgkhjtmr.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoofzhbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzvsruqz.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghylgadzf.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjlxvbc.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyustkoik.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggjhdwczz.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvtylradk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gltoqjoha.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gaatsabdz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaauepkl.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpkavrpv.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/ggxjzwbjy.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gureduybg.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gmcczxtuj.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/goaptopxe.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhmbmxhy.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gaescjdho.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gblqdlpsm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gghpyojko.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebiwdlm.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/guaxgrjtg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwlrdeee.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gktrtplvr.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghntvxifa.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghajepwws.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gydyjoiby.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkqbyqvj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gezbfrlav.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/guvifyvkg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaabbpoh.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gkbtvmkwm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/giahbidyw.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwccffcre.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gangxbjnv.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfcdruoa.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/ggbgjixoh.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshdhkljf.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/girprzwlq.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwyamicln.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gmczlefoa.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gonmxfcne.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gomudlxzp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmdjrzfo.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/glrfhdyef.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/glfjzswvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmnwaoa.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnaufdadn.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/goqylbdaj.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmogqrtax.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gafhdtjjd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymswjvl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gurysfafv.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gssyzyrwy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmgmiajce.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjocdpjp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdrmyqmhs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcdopbyz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgxaofao.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghurbbcba.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzcszykq.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmszphfff.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gsahaktjl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiqnyjzf.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkdpifui.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gocvsoonh.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqttmrazr.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqmxrdtb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkptbzdvd.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqbhgzfl.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmdobwjb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gipdhkuab.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutmqejna.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjbqhvws.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gldklcpgw.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gtkeogcmz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gujrgmqpt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/guiihhiks.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/geyoyjxme.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gebjjnhrn.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gttmidhig.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gnkjufhoi.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/giyxqpopl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdahatjv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafbqdrvd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gezxpvqhu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftpzzzjj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoqetkpx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gxmzufgaw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjdtqjxk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gancjycqt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gdroikmqq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gfzyebbzs.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwhfxtmr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gcocjkukl.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjgjbztf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgahncj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/googshdam.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtlsayh.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gcqaxiwxr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidzeupn.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gytwiwgqh.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gumhtqxyr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gafytxtkf.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhicujhg.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gefwosndv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gwqoxapmp.sHtML


<!-- 参考信息 -->