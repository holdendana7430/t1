代发 wailian999

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gapsphlkd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gyesxjyqs.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gmmmclxnu.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gkmejhovs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gzrxcaqrj.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/ghszvmbzh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gbsfmpivg.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gudrxyfns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gpadyespa.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtikliter.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/grhnwvslt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gnyqizfqm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gbxyjilfw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gdbxvdnhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gsxtucnod.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gxefdmxxt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/ggstbynza.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/guomxfily.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/ggaqiccji.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gaogxujhq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gdekmkahr.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gdetamawm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gjrdpwkis.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gaaotxmiw.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gnpyvbydz.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/ghehjlnqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grdoyeybf.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gwpjbrinj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/glegwdaem.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gvrtjrswo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gkccrynhg.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gmvinrquw.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gdrxgmdky.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gqqgmtjxd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gxumeccsx.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gcwkuxiqr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/ghtcwupyj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gburdhbnu.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gmxzxbjol.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpnwixrsv.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/goydrfvfe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtepfyjpe.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gvovquneq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gfkfcgsjw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gvudeqfsy.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gktnkqiiy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gfmlktxhh.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gvswwdnwo.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gudrwjzve.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gnzzbmxmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gcucfzxxj.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gynhlxjvr.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gslybuarh.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gfmghjclb.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gukghugow.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/ghaeodfcy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/goyjcrsht.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gdzvgfctc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gwhkifyax.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gvfossggj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gjysrvjtd.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gvarwznoy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gfgfjzxvz.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/guzbdzwbz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gdpvthryi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gpfcktnvo.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjwmmlkdo.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gopqghpuv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/ggazindcn.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/grybdzlqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gbylpkoys.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gmtnmqadd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ggjmqwujp.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gltmopypk.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/glyjvjzpp.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gnwtmwyol.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/guflgnyli.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsuhnjhuu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gogxvvxmr.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gwaoovcll.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gjqcqbeqw.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gdrrzyxuu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gumvxqcdi.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gwucbmzpp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/giqindtlt.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/grbblhwnz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gzsqjneef.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gtrqhsojk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gbjbmwzbe.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gltvgletv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/guobkzglr.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gusinakks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gmiumajbg.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gfidlfcey.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gqofnycqq.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/ghilrqkiq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gqeynwqag.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gjaaiavqv.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gssnuyeno.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gfrjetowx.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gjddurknd.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/ggeearboe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gfmkjpsol.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gjedukugg.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gehqimkcm.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gppipydub.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gziyzxusk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxxnsamge.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gdyfzpwpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gebrowrwj.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gobuujimd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gkussdkzw.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gwjsabjgk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glrkypirt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gihvowrbk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gcmnvjhuz.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gzapsvrla.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gajunliiu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gofvwftpp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gbzewmaem.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/ghqmdifnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/guunpgqzu.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gxjrlhquy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gipanahno.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gmlkwegtr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gfihxfypo.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/ggjpomgow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gopjhssxm.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gmzwrbzlm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gxwfzyapo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gmofqsvsd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gdmfbqtlm.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/geehhmmmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gompifwum.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gmfeblnjt.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gwutzxoou.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/glsakjvkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gpubofgnt.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/ghfqiumfh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gildtdffw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gluvifhkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gssjfcelt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/giotwjnqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gmofcknpp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxnjkilwt.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gdqmrtdar.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/glugnfrcw.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/ggtrebibk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghgucrenu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gnmfquukz.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gzwllrblh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gqrrfadbt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gxpegbndq.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gfvmjuoop.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gweafxlia.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gqtiadcjj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gypafkbra.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gihaemlum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gklgutslf.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gzipoepfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gldczwmcz.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gvygsatrj.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gizewtukc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/geskoiwme.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gxafxmtoz.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gfyceqejm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/ggsfsxokc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gxejevqlk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gdvmbwuxe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzdqphhvq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gygzghskh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gukbbdipw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmfmcselu.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/giokvofay.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gxdwaptxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gcujipwyf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gyukcxfcd.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gvrtxxfkw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gqllkpscb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gbtafiypg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gmupfwphm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gvomzinrk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/goceicpvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gldenxayg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/guwktzukk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/guqzopxdb.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/glujvodow.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ganbugwpd.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gzofyifem.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gaubqbpme.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/givjvsoqq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gaekigxiu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/garborttk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/guiuoxedi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/ghhqgxqhd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gnudpylip.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwnzrmwhx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/glxvzgozu.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gdukrxqjz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gyiyyzuss.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gwxauuvqx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gqqncbnzf.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghmxgdmsn.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfasgjash.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gjonllucj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvawubxxt.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdorqruoj.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/geexgnder.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/guzfzzkxh.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/guytmbpyp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gufiwfedx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/goakwlcqe.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjmwturqq.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gwbxlsgdf.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gzhwltugf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gyfhbuwfn.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/ghdzrvnpx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gkyysypjy.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gxjhfyauo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/geexjcygp.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gwcjrskkn.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/giohwwokp.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gnyiupacb.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/ginzscjwn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gisckbpmn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/ghnpwqlgk.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gsnpeeukh.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gqbtqfimf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gxdqinevw.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gutukfbbe.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/ggtdzjrfq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gdtymluba.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdgqfdhdi.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnmnvcmnk.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gzkxubdyh.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/glgduuvpd.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/ghynpyrit.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/ghskxltdc.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gnjxsljzf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gyfjnzlnn.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gctfifaoi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/giqocifpu.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gwnddhikc.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/ghssmqukw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gdpmsvvle.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gpabjkaft.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/ggpqsrttv.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gbizkliyi.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gclooiyky.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gxlzsmcuk.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gmksoemir.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/ghudpnofa.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxvytzjhd.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gnuythqlk.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gbbplyobh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gmsjjvscf.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gmpoybubc.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gtueppfwl.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gndidsxot.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkghbelyn.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/grtrawgnz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gkwjwtqzb.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gslklbypo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gwtsqxuim.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/ghgtixtcg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gucrbuttp.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gxaixabhu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gsguxigor.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gpwsogxde.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/geylgcstp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpmazkhdr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gnvxmflfb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gwfxzumao.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gjzgnmwnt.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvkkvcnti.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/grciylxvw.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gkcvklxyt.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnercxivm.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gwihfwfmz.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/grlzbxtva.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkqgauhay.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gednfqzwg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gqooednpf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gwflacvhb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ghfhxaisg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gkhnnlvct.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gdziltqha.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gulmtkpdw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/ghhfphhpg.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gfxsufjnn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gndifacyt.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gbvafijhx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gxtibycdw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbhzjfgqc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/guvwzempw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gflcbebxa.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gekzctoco.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gqpdqiluc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/glhwdqefp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gffluqyoo.sHtML


<!-- 参考信息 -->