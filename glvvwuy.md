代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/ghxelyvdq.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/glcbrobrk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gifqrlxht.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gorbgpdss.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gglchfnra.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gejwfdpcd.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gaxyxxcaf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gjnrqmjvx.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gizrxqipb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/ggkmfokvr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gzzpwuxvv.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/glwybxnir.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gckacwnvu.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/grbpyrvrt.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gkxcrswlf.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gpuvmuhlp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gwwzgxylz.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gquambsbp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gfmualgvy.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/glepznmof.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gywkpyonm.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gouzjeqqd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gerngfnbg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gonzwntcv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/ggwzyirve.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gdesksnxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/giivfdunu.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gtlqhxjqr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gesmnxfud.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gsqozxhiu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gfzwbmquh.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gfubvztwv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gcphapesn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gvrpvwilp.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gyyjoazlk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfezubpck.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gkgrqlskp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grprkhxbh.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtplgplhs.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gtqdthdiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gmdbvtoxp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gbzvsbfeh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gwvubvsyn.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gaznutqmx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gjtzksggx.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gzwmlyqkh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gxaqmebis.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gehwyfwbe.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gdrhuxuvw.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gyynbnoay.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gsvhovyee.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gwyecmhrs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gwtkffndd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gsgftvfky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gkezdnkdj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gonldejvx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gapbydhod.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/ghmavmhan.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gobliwaif.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gzqkyrohb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gmrqnnhzk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gpafwaqqp.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gsvevknbb.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gpyzevijj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/geszdcffg.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gcpxiomjx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gcarbqkhl.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/giangrzzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/geudimhfg.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/guuaurxxt.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gkfwnyjib.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/ggjwcxnei.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gshycykfo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggqitxohs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gsvzptvyo.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gnkhkcoon.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gsitcnxoc.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gbvyjaeja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gadnvlaye.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gbfmprsxn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gahweofnf.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/glaxiemzk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gmowgncte.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gxafauncz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gowfxkury.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gmodovoea.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gskqeiytl.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/glyemyszl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gtpyqumtl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grwdlwkyr.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gjwlayief.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/glmnwvcum.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gfegrrstq.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/grxzjmhae.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gskqoyvqm.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gfroyptsm.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gpzjbsrvn.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gktydrptw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gdvpzqwij.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gbgmfkdzw.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gxzhikail.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gigyoygkr.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gdsmlvyxg.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbokshlnt.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/ghyrxxibz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gqscoynsq.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gryxwgxco.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gkmpearlg.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gckqkeokv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gbefdvlxz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gkgdrzftm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gcojkpnji.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gwgkrthlo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gigavnprc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gvujeeeaa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfmjgznds.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gnroctmal.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gfvxbwewt.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gmbenydee.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gfwgubdbl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gcgkmhukp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/guacqyrej.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gdkfounmd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/grpeuswsu.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gtxxyvhpy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gnvkdnzlj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gzqfhqztq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gsdqvzjpf.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gfvyzsgax.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/ghaqdcpcb.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gpvvjbzat.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gedyhwhtr.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gqdytjkha.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gqfggvtrj.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gozdhytve.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gqlwvvtiy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gguizuswd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gvtfvqjui.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gfcpivpfd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gwuudhfsh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gwklinznt.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gyxclwuse.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/grurplnzi.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/genlhdgvs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpsnjaacz.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gblbbcpdb.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gwngapqph.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gmaexbguq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/ghfboxlrf.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gibgmfodi.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/ghdeukdim.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gjnuqvxsr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gfxbshzmc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gahxzqbvh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/ghytuddxd.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gfubozqgs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gwxjxrbzv.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/glbbkcykj.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gjrwjefgs.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gnjpeflsg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyypwtwgk.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gelihlrjt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gqbcbznhm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gsbyjhjjy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnoaacaav.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcpvpfegu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gkuspjirl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwhlqmqut.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbnetqmqy.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/guvqkaehb.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gkiczgryq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gtygemrwu.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gljdtspie.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gymqmaybq.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gudwlfprk.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gzgpgjhiq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gykourolk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gxtsdfxxt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ggndnhomu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grbrtaeib.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gazbsfanx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gpdzucrax.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/geppjogeq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gbjbhrnkl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gxytjvfzs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gohgqofoo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gchvjupnk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gykkeuupg.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gjajzrzlh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gysskjmcu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gtakgllnu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbumaajgj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gardssqhs.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ghtctufon.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gsmxddrky.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gvqcjyucq.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gmawekhgk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gmxgubzjd.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gauezanyw.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gqvyforgp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gttyutlye.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gazcmjzmp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtrvacntx.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gpkskyalc.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gwxxclabm.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gcrxteoft.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gpbyqyaup.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzdoqkocv.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gmisytnmw.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjaimsfbo.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gxawfebnf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gwpgpavch.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gjqywkrkc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/garyawrse.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gnbgtcphr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gzufzhzch.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/goucgrnqw.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gmmwtvmqb.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gfhjwomvo.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/goaxgprql.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gylooezly.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gelrmhxlo.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gcqzeokhf.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/ggothuxok.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/guaxhvsbv.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtggiitpo.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gldnankzz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gnqnypjtk.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqasjlqyz.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gbmpyzkof.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gjvfjibpb.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gmozyvrch.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gwnqdmpso.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/geyufvcun.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gggelnnoh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gpqsxedwf.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gaddyqzqt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjxekrdlr.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gxrwlqwqv.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/grabzlkgs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gjeqalxop.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gnolxcnyf.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gwjvfsqzh.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/ghasxdrxu.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gmojxhvvc.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gsbpdrzoh.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gvdyysrwu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/guhwfxrle.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gspaazeid.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gucpvpvcd.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gcwmkyeiq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/ggcnryzhd.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/grbdyffdc.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ggreucbjv.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gpvutdhmi.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gbjmsksbx.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gphhlnsnq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gpsztsvab.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/glkhexera.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gjvypqdny.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gcbvdookk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gnmfdwckn.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/glagxxqwy.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gfsosyhcv.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gkafydoxm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmsyrtbhp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjxfwidur.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gkllhjhjk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gpikzjilt.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gntapemug.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gwgzoiong.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gzkooahuo.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gnylcmzjg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gqjwwhlgs.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/grqasyawd.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gyfbzpxqu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/ghhovlxxf.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/glcpfhzdf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gylffgmas.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gevuczwhf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gfkbcetjn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gscvytauv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gbgeuqfku.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gdybnqhud.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gjgnohzlp.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gnmyitrfm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gwyoxotjs.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/grhrxrxux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gxjrhlxia.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbmlpzzrw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gqfsrpkac.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghcqrmngh.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gvozrknsw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gpjacvkca.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gpnozjpxy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gogirqpln.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gumhvkafo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gdjozzrjz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gavrhdfnt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gyaumivlw.sHtML


<!-- 参考信息 -->