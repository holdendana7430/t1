代发 wailian999

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdludadqe.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniyhwiqm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvjbxnzt.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopqggfwm.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gzvqnfzhj.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/geuwhpxrx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gbahypyae.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlqukzbh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gicetigth.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gmednfiws.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqgkkhvky.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggemcbyao.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnwoqbkn.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gfvncgkvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvpfaysvd.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/geqzlnquq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gotgffyti.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsrltnjn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gwizrysir.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyfvbvhw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/ggekghbpq.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ghhsvotmm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgafunhp.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gddvbjgtc.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ghxowgmwx.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqteqdivv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmucrlhg.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsnezksx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/galejlchi.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeusbvfo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/guwmtfxiq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuomubqs.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gabyqpjln.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrnmwxof.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfhvxkdr.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwcpipit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvdcovfxi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwzcrjuv.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclhjtbfn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gohcrbvpt.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeckearj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrrayqqs.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzwrpblvv.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gluasgoaq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttnvosqx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxthnvly.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/groypswes.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofxyxysg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/glezkvvmx.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdyzhttm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfzhnzy.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/goomqckep.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdspqclrr.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goovfavlk.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gddggahmm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkomqyay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/giuiqsbjo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gydiigoiv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gvuytmeks.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gxlbwtkaq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrugajjy.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrzdoztt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/givvgfhjn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokatohtg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/grskdlvmc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzarrqoy.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljhzbwns.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhplatns.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjskiddb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxmohstj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsflxbcuo.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykneqft.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gedrpqzws.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnltrkavo.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmlfotnd.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gmicjxwvs.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gbokpyozm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gyskgstcy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gphcpeihk.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/glwbqlmxb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtexuxqgr.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gckvzjdry.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjwpsrh.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuqfyiww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkwhkwzmu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvryijztc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/ghquozans.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/goxrlasim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkohoqotj.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gttashpvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpqzmass.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/galcwyvjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gkiunbdse.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gbmzcyxcl.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gdxksztvk.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucimmynj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqigoefg.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkesxida.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjzvamfv.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgtvlwwy.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtajsjfii.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gblpowtjg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gonmyjfzg.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gfmkltwpi.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gkauydzlp.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gcjxadfxe.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gstdxzufj.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtunznqbp.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gewjorhqh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsurpmsyb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghagvtnhq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmxgwkxvn.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmncsaug.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsvklxlf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gcllrabvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvuiqeki.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrhakowa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/giwrpuaeb.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gluyrsxnc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glaatgygo.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfbrwpvj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzpmepnh.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gifxqkcsk.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/glxfdmfqg.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/grcswjiyn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gsywhlwhq.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gtmlnsuhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmpqerpj.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfwjsxisn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcbnpyuhp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxubtjonn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcylbqzgr.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/goipbbejc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gwztibogt.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqzzxgats.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/guhirkfvp.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/grzhltjqt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggzidusow.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gibgjtzwk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxkdldub.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfnqtgxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbfulosoq.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmsxqjdep.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpminjyi.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goshakomq.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyoivgzbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gvcgqaoov.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gycypupsm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbkdcrve.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjnmdcbgw.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcgieuexl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdvrdihg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/genddmsfl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gpwbosbfa.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ggrnglxls.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlboscio.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvettybz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkdlkhti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkqgqkfp.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gflnwxuhx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggeekfrip.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiqlocak.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqgybdjb.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gaxippnrc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcmaglip.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllpjtiou.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gnjvqadvh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzjqkpgq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gpmglwwvo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkfrnmf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbvjrbc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpfffugr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grvmnmkpe.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnidaxdni.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbjtyla.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrzzsiah.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawwyzdpv.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gmzshsiic.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvdqdqmt.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkjeapqgh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvjntmwp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gbzdyketx.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gyskbbbxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtbjvntpk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkwvmxyme.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkztezwa.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqjzzkkd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvptjoie.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxoscxgm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoiteqhy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbzteqzja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbbxdayc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmpnistw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvedawoak.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/glqidxzmr.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfbweoky.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwquouzd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyjmhieqh.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkcqdnhhs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbaxeatw.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gzitjycli.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfpocuqj.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggangmmfx.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihooyidc.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grsjfxlfu.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcadxozz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gljldpqwv.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gigmzlirz.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrqqpzcv.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gcavttvdq.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gvheipamd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiffwnqt.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvgbbyrp.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdbpdgnno.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtnnfbpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkdrjfti.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gytekawuu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gykpyitus.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaevlctqx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbddodcnc.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvrssojx.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhaiiknw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxeawsjr.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gsvvmqwnw.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgafnmij.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghemsvxue.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gbhbuthpa.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyipjlufb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gmmrmdipw.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gjsqnlmtp.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwvcxcqv.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtnatrjhc.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/greyqivpq.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjztobol.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpdqctbd.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gsifmsasv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjavrikm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwwemcwp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjjzgwgj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gunrfgdyv.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gsivtlcie.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxsdbdsa.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvyswobxm.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjimdgenx.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gwihnzhgr.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gpjeiwcvs.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/genemmize.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjycfurr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gryrzddzc.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gffpsqqxx.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbefekxvd.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtrrrtuf.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjelwhofc.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhhcdlnp.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/guaxxunxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhcssvca.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gaptjcjix.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsiaarfs.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyphbbjww.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzdculwoq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcgaeuikb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyacruart.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/guzvcsyik.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnlmhmow.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gwdaabphh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuaejhfp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwiduodu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzokicbsf.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpunuoch.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkaedwcb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gujigvtdm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gcamaimwu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/glnogudjf.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmkbygau.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjyddaqp.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghytmxsbj.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpangcifb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/grvutfnwa.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjllufwr.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gaydqevhs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gecsxxuyh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gljmncbbl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfllujejt.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gsdebtxfj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgnpqnne.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxmdeaw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxuoflu.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvryyifyc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjxkjzns.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpbmfpndf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfgdcxhw.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gpobkxmab.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyfgznnz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtduuoxfx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giuuvwnsm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gutlufgph.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/ghxdvebkk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gxkltgnbu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guezdrnuc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpjdtubhu.sHtML


<!-- 参考信息 -->