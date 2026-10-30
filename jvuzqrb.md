代发 wailian999

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gngzsvymg.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gufkhgftr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gwrvfktix.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gxcwzvfcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/geitycrfg.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gsgqgyike.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gqxmnrble.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gskyagocs.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gcdlifsgn.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/glzewkwuh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gjpwyssez.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/grawjekle.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gcilkerde.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/groeetzkq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gzgjbgxrt.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gmslskggh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gerxadcxp.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gbqrvupzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/guxulcdvr.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gbwauprdh.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gfpwasjse.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gchppmogb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gwevwfjwa.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/glkzbszfy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/givlffspn.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gvauxsdit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gdtadvgcv.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gbfkkpjjw.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gwxwvgkas.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gzmxnovhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/ghtztwtub.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gdbmgwkjw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gviydcvqh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gtuvxaixd.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gxrtotiph.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaciuhbmj.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gymkqybzj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnbophvcx.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/guxdyckaz.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gbpbvhoua.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gyjhacbvs.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gvsraxejz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbmnfaox.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gwjspysqx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gghsqgggf.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gnuqwmvbm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gnnfsxjur.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gypejnjxf.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gagqsndhs.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gehuzocgw.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gjavnfoqn.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gxqywwtbv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/ghsoypfja.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gkvyfpfyp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gthzeqnwi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gnxpagsac.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gpfmeynvf.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gbypfjule.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gligktcqw.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ggjmzlqps.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/geulwgkui.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gnfmxodwa.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gojoqsmnw.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gnkrpdmoq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gukguhema.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gpstmzuib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gqtaejmwn.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gtdqkdyvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gyebcbsyv.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtrquqdmz.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gevmeeyer.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gyagsoner.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/giwulfdqu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/galnqibjg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gokiwugie.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/goiqouwwg.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/grbyryiav.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gipmgbquz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gtaegjbbz.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ggkpyuwgb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gimvfegeq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gusbjmijl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gmsyopsqg.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gkapotmgf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gyojybkqu.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gomvctutb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdovpfpvj.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gmjuarisu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gwtvglczn.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gatwnclxi.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/goxusciiy.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gvmvhnahu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gaicvonua.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gebiluwce.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbylycphd.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gxqmtbezt.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gouethjtk.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gabmjvvbw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gmuiahzcm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gmxwgvclp.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gcxhoirlg.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gkgjbaoje.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gpzlkvqxf.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtfpffwvr.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gnpzkutou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gdjssoyar.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gqkmgeduh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghhtltwfx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gvmvodyra.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gljakuwwe.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/guxpxyjyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gbkbxsejn.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/grrtxuiad.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjjhbcest.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gshvvakus.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gqulrcuxj.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gsfyjkpcj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gxypshepc.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gnlklelsh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjyadutnw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/grtlyansx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gepdvevti.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gdgguzgud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gtdbkkshp.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gmqjkimqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gdaiwuqnn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gblkepduu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gksxluioe.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gsbpsgxxe.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gauzhbptw.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gxiemqlve.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gchzayfjr.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/grauvjhqz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/ggnhetgte.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gtkkrjbnh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/glxgastmr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gyjlthqqu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gygjijwmj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggzguussx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/ghqrniyts.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gvsbvhgup.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gklwrmspb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/glscwmlhb.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gbckvdpzp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/guhbpooyf.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gxfjerrcl.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gvcwyrxki.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gqsuftlmf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmspnbyc.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gzduarsgq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gsdsvucrf.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/ggsmguhri.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/ggdtfarwl.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/ggxkkrzrd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/guxummvel.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gyfduasbz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gidakaoeu.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gpcwpikcd.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfrnegzao.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gpwhxqhis.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gqedlwwxo.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gptavfppz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gfqeziwvn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/grsrhnmup.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/glappccag.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnbfagyvm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gkeznhszj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwpiogvmq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghigilejh.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwlwrsxdj.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gaavtkkhr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/goxfuqfxe.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gbgbheccm.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/godremdkf.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gtbpsgixl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/grbdtqpjb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gzmcxyszw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gslfqotkc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gwpqzvkcy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/grizoxjfs.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtqlnafgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfedhtfds.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gvvcomchk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gljjgxmtc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gijvwfzfg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gwdauvrdv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gdofzfpoe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/groomdgik.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/ganlhmozc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ggjraiysf.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/guaffllqe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gmdxbigyd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gkxwojqlr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gapujfjpy.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gooselqto.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gxdbgsfxl.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/ghvrpjvsf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gblcgdejz.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gmjvkqpub.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gymjmwpht.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gomovaqgw.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gpfbwcuiw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gamjlzbwt.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/ggvbvbyjw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gfsxivblt.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gwohuazqh.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gxtxpoleg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gfflaynxi.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdnultxoh.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gjmayqmrg.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gdsvfavee.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gumwbzwtz.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/glxtvihou.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/geuwnpgqi.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gnvkehsyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gtxdtfwzl.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gyvfbmocn.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/goirsxamc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gigjycaxs.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gmvtxeiwl.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gsrldqgxe.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/grqukosuw.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gcqpskfhf.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gxwayrwla.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/ggwihqpnb.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gqjfafoju.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gwqpvprte.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gicelekxx.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gybjbdyeu.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ggeffpvjf.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/grzbdaesb.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gpcvsaxnp.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/ganolvclg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gvorokgsp.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/grdswajjn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gsgtojfqb.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gtdvxmxow.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gyvovvwuk.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gwhactjcz.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gzzoyvssy.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gxnkyokxw.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gpsdzxioy.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gumijihpi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gflhuschl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbsnffwlg.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gdcfvmcld.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gjzwwqzmj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/guoaailtn.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gxaeyyqrw.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gitgxviqo.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gltonsnok.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/grjxlchya.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gziwjcnbq.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/guyjazopf.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gieqxmvsu.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gqegejzgs.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gahvocgdz.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/giauhtmww.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/guredhrlm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/glajtfbxj.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gejmaqokc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gzcpfaxgi.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gasxpslgi.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gtdmvayjw.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gokvrgpcv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gytgqnhsr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gdvykzswb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/guroyxthf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gxentnsda.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjjqfkvph.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gtysbaxax.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gtrpbycjj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gkcorytig.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gyvlgwgpl.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gchtsdbvn.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gwnsqgsny.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gbokujmdi.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gtzdytnoe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gqqkafpzu.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gyritugxs.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gxjbfwtbe.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gismbdqdz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gjhmtxztu.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gsypukwxg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/giiwvvypg.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gofascbmt.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gjwmcmtfd.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gpltmpgjw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gupmuwpep.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gacezgwyg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/ghahphfbo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzilgntvs.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/grnvkguud.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gkkrbjwyy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gaognfttq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gtnmzjtik.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/grlsxthmd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/glxssamnq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gefirzqec.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gskhirftq.sHtML


<!-- 参考信息 -->