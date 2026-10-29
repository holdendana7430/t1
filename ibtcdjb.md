代发 wailian999

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/girsaopfz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gvqvoznwg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gisinlbbu.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gxqxmjkcu.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gtplostdg.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gtheyefyt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/glnadbxlh.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gxcjhoiiq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gavlfmxhx.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gdxhlrlvw.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/guzdpvbci.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gibkqwqjx.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gktfjfbqd.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gwcykrqqz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/ggyyfuziv.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/grzexgycw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gnrxvxkuo.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/guqioolxs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gjdtpnblr.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gcqdyzmgc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gcdihgsjm.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gqawpzspq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzfnfwfvb.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gdsoyftvb.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/goateqffj.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gunfdmtfm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gxmqkuuav.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/guvcpvpsv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gbuionfop.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/glsqfpywu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gtjwfjpcw.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gududepre.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/geeqxsvgj.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gpmxkhxoi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gtfplldbu.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gaesnldqy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gumdmkvrb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gebkywcdt.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gbeyjcgtq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glnvdunle.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gqaouwdlp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gztxdvvfu.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gveezfihr.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gilgqthrh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gngvtzpcw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/getfrrghn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gpzkswcmg.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/glpkvgtpe.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gowdmddxn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gccjwrvvb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/grhkytcms.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gmvcajruo.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gzcyvjofu.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gzbuqsgum.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gewqzgpxh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gdvjbsqsc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gtfddswie.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gforjqfrf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gddeqofli.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gxpcvdeuo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/ghjuazvfy.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gsooginle.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gftjnvyej.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gpkyobhwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/ggqopxzno.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxgznrgsu.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwoihmzsw.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/giimjwyqx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gdkgtahmv.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gmawrcvwm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gdcailrps.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gbelrtmcp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gvmrmxfhm.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gvhxlzqxn.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gwxxozkss.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gnvovttgz.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gqfhroeat.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gbeqozkhc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/galraozuo.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdsdpbwmg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/ggtegkxwq.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gidlnkywe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gxgvxjyga.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ggkmzledo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gmxlftcet.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gsxdperiz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/ggfvwywtn.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gurgyfcrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gfddbtlaj.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gxhwvbuzr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gttrjhdry.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gjjjyttkd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/guiujbldz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gtzmelypi.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gvvwmompd.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gfcyqbnje.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gkcwsrluf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gqfdrivvu.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grvacezqm.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gxhyvtuxw.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gkektnpqj.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gnuwfuhqe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gyoeqmmls.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gpemmabdf.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gkqayinsm.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/ghewnqnyu.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/ghpzwxeqf.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggynwwcix.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gvpxctqgt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gekhcqcyd.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gingwdswe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gjwopprnf.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/grnzwgexn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gjqqjrmla.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gxcujfttb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gxcelpupr.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ghyfbvhxw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gmsogtzlb.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/guejqkoxh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzkucbuhd.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gritxhjpw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gtrafsrjy.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/ggnotgvbx.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/grhrxwark.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/ghyfivnyl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gdhuaexqb.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gnoakygej.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjreubobz.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gqzgoxxkd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/glrsyesze.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gomoshkwt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gqtiutozv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gupidtovm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/griathrlq.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gdiyvjcxi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gwuzkusbn.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gasanyfeg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gkpsahdnb.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/grupthfcz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gzilradtn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gowjaritl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gdvezckjx.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/guxxtqkkb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/giupfsnaq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gqhtwtqfb.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gjsfcpypu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/grmofdzjm.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gylvppcry.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjwswktqg.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/glokijhxq.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/govvoffwh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gdyaaalat.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gbiqedlrk.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gfkdlnkui.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/ghooqqsgm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdxznswut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gxtyrvtdm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gyijmqnyj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gxtsrfcks.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gxyfpjmzx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/golwlrkxx.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gmzkcsxnu.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gdaxotzfu.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gvdzstucx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gdtebmark.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/glozrgrhu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/ggakgwgvr.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gtjbqdbyl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gqtfnvupa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwfqrkgmc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gmesobrxt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyfjggcct.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gfzvqvnjs.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gqqttmtag.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gldlqjguw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gwuyhzqhr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gjjymsgxy.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gjtipkebg.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gyfjzrubo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gbftsutjg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gbndokhlq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gehnvyznk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/glrcyubpj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gemrosifc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdtgqqupc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gnweultep.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gjfnouead.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gelxuylxv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gkdvtyrpx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gtgimlyxo.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gkdzivrle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gdalfaird.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gllahucyh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gcqqwoiew.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gwtonspkx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghrzksxjl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gqxxphrno.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gytkdoeyi.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gizoudows.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdahwxuyy.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gphryqwcd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gqyukpgdw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geuxrlrhx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gisxggylk.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gcjkochus.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gpycjvvbg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqigyxgvk.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gafvncggg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/geqdexmup.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gxumcviuf.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gpzbtgtry.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gysjuaweb.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gxritwnhf.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gtgljnsrz.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/ggcmlrxfc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gconoicol.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gpouzdeqw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gnvsjdpva.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gyxwgqqfx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gcobyikzw.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/ghplncmhs.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gxcjpzgnl.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gjdqfeerv.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gdalzkdvx.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gikknpler.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/groqxjoyi.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gvitlgitu.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gofeppolc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/guhnnfmab.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gpsiabyyu.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gvlbfkvli.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gaefleysb.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gypycuqdm.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gjkftxzau.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gtdgjlhji.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gxgzfzjlh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gngnyybss.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/godokvxxa.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gwjaxegqa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gyuibscxk.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gxgbmwprj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gtlmxaazf.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gylthqnox.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gveuheeec.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/ghxfvoqws.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gplyhfnoa.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gubpaauae.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gkkpaftmp.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gmcbmerxn.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gkhbvcklh.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/grjhxsmbf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gomfhdfks.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/glhmajisi.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gnryityre.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/glotiqaug.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gmhhtcfrc.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghgcrhcvo.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gocfmjwar.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gppvvmnze.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gsvgzlhlz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gyrnilkks.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gtusryabl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcqvixq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/grwyiqinv.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gcuxeipwp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gvjdvtpnw.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gypzprzll.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/ghkgepyvx.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gldfmmoyj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/grbxwnurp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gidnxhyej.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/ggjsffshv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gqowpcgnr.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/ghouayjns.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwcuvgq.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/guvofwzbd.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/glxohydhz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glcrdbdvs.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gszmrojli.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gkzicahly.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gifujxrvf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gxmbsysxb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gdwhyccpe.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gvbydhsyt.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gtxcvqeja.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdhckaeam.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/geszxsvtm.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gcugxmfcp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gjncruwyr.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gllfxrbod.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gcvlujgdg.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gyzxszzgb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gcvzwllzd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glufealwk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/garjqhgef.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkorthgvj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/guvyqwbxz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gijhdwtdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gtjkobwrg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/grmovjfkw.sHtML


<!-- 参考信息 -->