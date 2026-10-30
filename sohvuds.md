代发 wailian999

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gwgwcmhrx.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghnodwcaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/greqwqmrc.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoqrcsts.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnkfzsex.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjzfqezjy.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtgrndnly.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gdygpuiad.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdvkytgi.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gosuqbcvy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpugrwycd.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gvjaiohea.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gepxitfpz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhqvaea.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gjwkrxzjm.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllsbzllo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gynuddjeg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmbtqbye.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzdbtaps.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnpvtjovg.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/ghxyebmyk.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxbdvcpg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwoywrve.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzyqpwcs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupkhnqsa.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaoqlfrvu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbxbqrwi.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gharzyujk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiftfqey.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaoyrkia.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmiqextsf.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gcvmuibwb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbqztcrcd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gieirxngf.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdedngim.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjvlkdwx.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbokvzdam.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghfzwjqln.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gumgjvael.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gumeffrqy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtviqdaf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gskblxbsv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gvgofpyqz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgpcoda.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbefvjzw.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gytibjxcg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gungcsooz.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzgpnegam.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfeytfjez.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclsgkbr.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/ggitsvpbe.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvbeuddm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gdngesyfj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gprfynrso.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqcekxki.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/goavvtgji.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynryzcfu.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrrfsfkg.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyxngfud.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grwpuaxwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzydrrjbe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gviwszclm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gofrpesvw.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gldxwkoyz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gngbtwamf.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gelnrtbfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrlwgfpv.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmqlohdh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gtzeyoamk.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbkohvfuz.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlmoblwt.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqbvggyu.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfxmmbiv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gspcjkjrs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/glcbnvksm.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmfinazl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifisorg.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geytldhqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgbmiyln.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitkrtzox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/grhnpkval.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gqocnjiom.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gabmqwsey.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfyoixasw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/greywtzjp.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gihxkguvt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqyifcedx.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/grtrnrszb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/glwogksmb.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gfihioabf.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/geqcjxbfx.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbmbpfh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbwbdspka.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gnwtsczyh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guozfxafv.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzsgivgo.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/geyucznpd.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtbxlhhre.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwkwmbldo.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gguhmeksg.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjqicyp.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxddhuh.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggkohgksr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcbukucf.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/guqqkmffg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsdyfafda.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gepbridxu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpodliwbn.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gakjdmces.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gqebqiqgz.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gygpqkxxq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/grfhojfxi.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsayipguu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwceecgiu.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/ggaziwnxm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzktvjnl.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/geddkaqyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/glvtkcyoj.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gubczwdka.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnyqcvdj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbspeyfju.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzwbvtkf.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvngcxwr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/givvpqifx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwvppzsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzypzucg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/guqwwvraq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gphbpfxot.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gxagfirae.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvtnblor.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcwtrpum.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guauocaun.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexeihlx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/geiokxitx.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gxpuxpnuf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gytwfmgfw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdxxwzcn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtervckca.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gubepxcrv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntnwepyo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gycotjtmc.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guudaezxa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghutgnwyx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfxjxpda.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/goucyjwzy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlhkhoxr.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gxwzdgiwp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/goefqgame.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghlpbndsg.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjttjvays.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gowdwepqx.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfqcmvjdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gohijlnpj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcwhbzdeo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/glthbpwmx.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsivapap.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxrtgukh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpvuvait.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjtcqrbrw.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdircklw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gqitpgeeg.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gyoidudkx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gbtlrpdkx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzctmpbz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gziardpdv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkmjwwfx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gmcbowniq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvryyrsop.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvxfrlis.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjhbfgdw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcioyqj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gwvcnshab.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjsmghyt.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjiwxyizj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuhqqsce.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrnoaobq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gneoxdqji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbllrdfze.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbicdwdrt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnokwpvg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkztptvia.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbadgrlxr.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gimhptwyl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcjzzelv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkxwwqdh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqjcxsc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozvkcrko.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpcuepyok.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncqodzkh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gfekdenuf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvveibc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbliopkz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjwyorst.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbgrztly.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gesmqybyt.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gripjgqam.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gkmspkzxr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwijbmut.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkbpbzgl.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gleawojmg.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gamrwmcez.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxxomaucl.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccjhyjk.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvkdtzmp.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdoekrwu.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqjqlvazk.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/giafkzxmb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gycvvmmww.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnjobvqr.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gagvnryjr.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotmxtiwh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjetyfzi.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejzahhs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gfzfmurgc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqhjeern.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmxzndvx.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbapuezgs.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgyndlf.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/giciexzjs.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcausydqb.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuskkdok.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gowmwjaay.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnubkqch.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gfkkolwbs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/grosngttq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpvjhknq.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gxlxdcypg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmrwmubg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvqbfcuz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugpgfqd.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsszwzmzd.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/guaxlyzyo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfitfylw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/grlldqigp.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gnofnqdrt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneoofafx.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxpzpnyn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goyttlhgg.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwgqpvzq.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gtukmabql.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvjnltcd.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjstftqt.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvawcjvty.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzajvzqxo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujnkntgt.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytmcjhmo.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gwhvkiqur.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gypghorvb.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwzoama.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcayacgzk.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwemtkrok.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdvktxbo.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gyzfwlfqq.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gqjxhplmv.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grloaaiwt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpmvfyph.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/guqmihzpc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqzubqbe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsohuguzs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gechtmour.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznuecimx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahbltmxl.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glflpsxvj.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gndkgioch.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnuhlyquh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gffmefryn.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gugckcffu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqizgwwqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gczingofh.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/glqwqfjcy.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gdzhqqjxo.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gziqcbeqj.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrhpqgwq.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfktenep.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbziyjvq.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/grxtyukpe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmhtcyhd.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gsayoymam.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjjareom.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gxnvufsob.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujktchfa.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gcflanjnd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjttyixha.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqktueplu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnadscyd.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggfauxhzx.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffhvbvyw.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gfmenbpip.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqnxevpf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggwthgcuj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/godlparvq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtorgrsmh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/guxwigkgc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwoyztmx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgobmufe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gejxniswr.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsmwrxh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbdqfzc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/giujoffsi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/giqdyztjj.sHtML


<!-- 参考信息 -->