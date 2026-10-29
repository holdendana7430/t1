代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gtxsmcgoa.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gtxlgfvcf.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/ggqekhmzj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gaoxpdima.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gdggtntfo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gbmzyizsg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbbukdh.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gngpmmnbq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gmllmecht.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gphbaywgs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gypfrrrjn.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gblgklfgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/graoqnxbz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gnyecopde.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqlpzcjoq.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gyjzxusjv.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/grvzgeawi.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gxlkmbzcd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gdkzvyykl.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gweycrdcq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/guqxevljj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlswlsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjdiklcet.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gueuzzmoz.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gauyacpnm.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gzcygxhbd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gjzefkatw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gdprcsqbk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gcoupftqs.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gfonkgdbw.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gpkozhdjt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtqciyjtc.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/glkeqqzdm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyhgsqhgr.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/grvezfnat.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/geovsempr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/grqyvdwec.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gvqwaczdk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gqqzcmtvm.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gqwwjgkcx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gjnxxucor.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gnykoqzyp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gtnmeinfp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/grcgprtaf.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gpgaubugs.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/ggdjcffco.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gjjcrcnmb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gsaiscljt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gprvjxnxs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gsphiuxxm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gmiutfljw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gnpyohdxd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gktkumhpy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gcugkzlzk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gmciyvnec.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gzobohppn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gsxkdlmve.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gqbxqwvci.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gztsheejo.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gwoymymvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gwrjwhsrk.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/grukupmvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gyotlhkvz.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gstppuplw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gtahpvsow.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gsythgoke.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gujrfjgqm.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gcuinnomg.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gwnlqdddb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfczlttwr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/grkbvdowj.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/guzdoafiv.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gbealkhvf.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/grkrwptcf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/glgkrsunm.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gppqobstj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ggoridkjl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gaesopeef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/ghanuakms.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gjrzufpov.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gonfqhwys.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gdxrrebcy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gxvqgcveu.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/ghzppzirp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gqbklneem.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/ghiuinzqb.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/giptbrwbl.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gpkojiqsd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gyqsmlgfh.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gnedkhrvl.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfuglirfs.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gpaluczfz.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gxdhshojs.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gzsufskzj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gbjkthjtt.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gdxkqbtri.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gzjvtugjo.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gedsrrpbb.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gafzcurfj.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gsgztxnud.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gaepvlpyb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gkyiqnuag.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gyxpjzroi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gbxeihubl.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gnlnryibn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/guqulcdny.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gxqoryqnl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gbuwrnwrb.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gkelvultg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/geebpvfih.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/giokayziv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwutyxqcf.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gpnrdfink.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gttmnlfsd.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gmarsgick.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gxbftqypp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gneyzfidr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gcuwhsmlk.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gwbtuapqp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gzggxunby.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gnbujdxhl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/glyazdbok.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/ghwcyrugy.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gyfcibocr.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gsydslzxs.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gdjducraw.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gfkqapxae.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gvgfvsqyt.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/ghvkvhizu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gblzlphdw.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gonvacbkb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gjkvnwtop.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gmjixsmjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gyptnxgit.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvayjunru.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/ghqwixxlt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gtamwmirt.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/ghaunqtqv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/grmyjivbw.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gwdjhtarr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbmitaasu.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gqxvgrtdj.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gaymqsjky.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gjsndklhi.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gfgozvtrw.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gkrmyqvkk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/grzsywjax.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/glbowgtmx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gpomwhchn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gbmqbwezr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gazdhrdic.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gulovbuup.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gvsqfquwj.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gltbvcciv.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gjjmpedqo.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/ghzwdcrur.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gavyjyerw.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gmehqyirk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gfdoahiby.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gfpbvnzyt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gminsyqbz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghmyzjsse.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/galavklzu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gymnrhpfr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvjvwqxxk.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gvqtwscjp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gapnmmwij.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gtmloeiyw.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gbdllawwm.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gaupoftfh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gkevknias.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gdwtmetkv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdvmpcszj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gjupxxija.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gicixmxcb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/guerouetx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gyzfqlelv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gologidky.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gqvqvjoov.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/ghzihelqr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/grcfyoaec.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjjkzjj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gbruzcpni.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/geeqavtbm.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gqozptwyp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/geldvpniy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gndtkihgw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gfgxjfpgw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/giejiyyca.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gbelgdxog.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gdpgazedv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbdkxjk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gdsohaisi.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gomhoxksy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwtwmqbla.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gceajxnpt.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gwktvsdtz.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/ganbxhhnb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gbukhaqkf.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gdivferhl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gqqobtfac.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gatzgnvah.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gpbrrhlgt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gvcalzgbo.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gepmkeiat.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gczdcgwny.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gvuvihlnb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gfjksgiul.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gtccnigwx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gfzqepyvz.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gesebguap.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gyooednjo.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/glvnbjsxk.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/guvdwfyxr.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/ghsgemulw.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/geumeybct.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggrhcxwan.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gnjblvsno.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gqyvalvfb.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gnajjptiw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghwbcejch.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/ggwhrfovx.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gccnjdkvc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbvrvyz.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghpuaonav.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gpoulbuun.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqbuhfv.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gkfzmhkxx.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gzvflwtsy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gyhpwhfsa.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gonclukzw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gaydqvdnf.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gezskgfug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gslvfidvs.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gnrrhissy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdzktuj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gildzvbev.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gecgzkoma.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gxwpjghld.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gngcgtyqf.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gtwruzdjz.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gxfuzhjcp.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gscygdxih.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gjiluxmic.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjvyzygdi.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gdrlbvydq.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghtwcykcv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gofvkdvdz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/guylguhuz.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gwbbpbrvg.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gxzaqhwgz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfejntvh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gqkcxyvzx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gvdcdyghz.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gcqnsghxi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/glbhicuex.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gaudccjfi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gppcmwigr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/geaincljf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gjvnflfez.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gtutdkann.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/guzutmego.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gbltwpjjk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/glhfopbpo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gcuvszfsl.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjipmbktk.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gariioxbb.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/ghonexdjy.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gamfefcbd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/genijljec.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gfvtqxqsx.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gsbldtkqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gknxkrvoz.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gcvyoailz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gcspkcaxw.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gxrnymboi.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gjwpuskib.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbuhjqbwl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/glpijsgok.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gfmccatwl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/giygzmhrx.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gqdcubtzt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmguwtxnz.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/glpbxrgne.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gexapjyqs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvdrljoa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gkfzuwssz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmjkyvxgd.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gaofqjksy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gujqlnadz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gietewtvr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/geusueqre.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gavupbocw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gtatsrqpu.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gevlftrza.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/ghysxuxye.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gmqtzremv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gfvvbbjgi.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/grmszzzav.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gtmyegiiw.sHtML


<!-- 参考信息 -->