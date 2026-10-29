代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gvfbuhazr.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gplbvwujl.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/glhggswov.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqyzybwyp.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/grprofgod.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/guyahwmjj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gkgnjkjdg.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gkeqdskbw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/glahhxlyf.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/ghuunryti.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gfdnvdvyu.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnhytartz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gptamhunm.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gfnlhbnnk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gadbndlrf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gwstrtxnh.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gihokyowl.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gkdulebfw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gqjvjshzs.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gmgzwtbum.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gkrtxycwf.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gxonhbwpt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzanqjnop.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gexaaeizz.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gbvxpflxi.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gsxellkdg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/ggxvkklhm.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/geswgnvff.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gzowyjrxd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/giiybzrtl.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gfulzdbek.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gneyfmpja.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gtpbvvdsr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvaleprni.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbddhwjql.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gltrhtloq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gxshewpor.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gabfugihw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/geglzdvhm.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gelhxqdvo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gfrweysba.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gujgjkish.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/ghjknrkfr.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjoezidgs.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gxnisfbzf.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gcdksdswl.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gaafpubnw.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gugovejpm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gzryszysx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gmhpzgxuq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/grvlkqvrn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gaaendmqb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gxuplyjmh.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gkfbphmbh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/ghmmluqit.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ggaymfxpu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gaeazmbzr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gqznyjuyx.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gvmifrljd.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gqtjbgzrd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gouavhotn.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gvpfwbfuy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/ggwediddh.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gajjbrupd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gegdmadaq.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gnefekkik.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gnwuhfqyz.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/grzvdvcml.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaxtkxmnp.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gkmmpttub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gvvogcguj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gaphelybi.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gjvlblevg.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/guoxokgzu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfthcddrk.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gdbikrtkq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gtatwaiql.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gcponrhkr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gabqpejke.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gddgatjux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gnljdorhj.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gklfurbyy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gaogezjcr.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gmuprduiu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/guytljylk.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvlzztwrt.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gdfzavohe.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/glxoxjapa.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/glikqupkg.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gwkuowqct.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gelsndrgn.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gxzfaibdl.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gglkqycfd.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gykssylgp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gauozyrpk.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gnnuemkwr.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gvuljyter.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gnncwpqne.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/ghuzxdsgu.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkvoixlyb.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gbzhpizux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gytcyvokb.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gxuqejprf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gtbktygzi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gxhghjmzb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gyofaxfzk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gwkasbmcy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gecwvqoav.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gjepglcgx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpaoyoghm.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gwcmkdfrr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnnirzhtu.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gdxkrvuwk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/grhxrccwp.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ghlmwuftn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gxppyrnbg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gfzhwhehi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/glxdedvrw.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gnfszkfxw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/groosvgrd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gitmxtqho.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gkbthmqdy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gfdirfedk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gklglkras.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gbvynrybu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ghbskzfrt.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gotjtadlc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gixmwnhcl.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gurkljzyd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gzkvmysne.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gvvvathgw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ghbjgwbnc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gkzgtgque.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gkbjoojlm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzxkgqshd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gkmtvzwnf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gnbkkepyy.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gwtkhxqfk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/guejeonof.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gwmllwrwy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gdswczkwe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/ghjtlgiev.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/grcyngnqw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gsurbsxsv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gvogjzovd.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gugbahwai.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gorhpvzob.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gjftcankl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gioawawgv.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gxoniidqp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gmrphgzta.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gazgtauxh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gjxzqyije.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/garwyulmd.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghmjzhhna.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gyuvbpabq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gzobkmsvy.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gjxmioxen.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gjfoxhrop.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gcxjnhaip.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gcsgxbacm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqazxgawe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gvyoigqfy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geeoscfma.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gewlddski.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkemeejjo.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gvxaivkvw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gnsueyjfu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gdckdbmzj.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gthoqapxw.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/grmcimtqc.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/grnvpdjdr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/ggzebahbi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gtmhhybzk.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gnxvzoqep.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gqhykwrys.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gmfcjouji.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/ghwmzhgud.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gvndsggkx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gpdkpweva.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/ginazizxs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/ghysrijke.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/guqtzxnqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gazhszily.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gbtgnbmke.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gqrjzmpsl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gppihhocl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gvgsbgncg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gfhfnqyuw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gxztljqjs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gntkgxuym.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gyjztnuhd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gwpeysgcu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gucxspfpt.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gnztkgwxu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ggnmyoane.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gyhuonvtd.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gixvcwbvl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gjqdsegus.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gtzkbuxhv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/ggumcrdmf.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/ghujbqler.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gyjywfcbz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/genzupedh.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gywotmjhn.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/glxjaemxd.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/glavskymw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gsqrrvxoi.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gezbpdhhb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfraigryz.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gecysbrpl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtyrzoaxl.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gcsiovoti.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gnglywtst.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/garjhaetf.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gxykiqiwk.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gjalxgwer.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gnqzaknny.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gwmlyjxnx.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gttonuuve.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gdlalebbe.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gouggbhoq.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/ggsepuwjj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gxhsuzplc.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkhlkmaxa.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gaspnhtwu.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/giogjkayh.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gvpouqkqi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/ghemlzcfk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ggltzeeqw.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gvznkyldr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gihmivujo.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gkkmkfqzi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gpnacqjfe.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/grbwwdlig.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/grmdsocnd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gpnvmwrzf.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gpjbsdfds.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gngdivvli.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gztotdikl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gepzszqth.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gxmbcdnnf.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gmkrtjsba.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gtynfulus.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/goriddngf.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gkdohrszh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gixjgxjam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/geassuahd.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gaimudtdy.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gyojbfvjv.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gtevekhwz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gnkoxkniw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/grtmehatq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gwoxdoixm.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gwnkgsmld.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gybgrctnc.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gfpqiqoqo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gckqfyoeq.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/ggfpbwwog.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gfxwjknoi.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gpopubygh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/geefkcglh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gpftqmeli.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gszbjeoaj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gmjuyhoni.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbitozwqd.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnavuccrl.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gwyobelyw.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gbtpaxaho.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glmugmrux.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gklrbsvhf.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gpksugnma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gpvnropbe.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/grnpxpqtq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/guwaybgqq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gqzivsdjr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gsbkewdzg.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gnwospwgb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gbxulrzdo.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/ghpqeteky.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gcblguclz.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/ghatzcobz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gwcegrnuw.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gjgjdlraw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gkpyvovrk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyynvlwgf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gpfjqzdlw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gousixxdn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/ghsnthtky.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/geyyhrjqz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gwflbnztq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gossiqpbw.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/guetrcdnp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gcnmxofpi.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/geitqfkoi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gsttpdqnq.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gptfvjitr.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/giltlzvum.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gwvbgkdpk.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gheiuliqh.sHtML


<!-- 参考信息 -->