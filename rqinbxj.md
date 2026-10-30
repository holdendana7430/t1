代发 wailian999

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gowzoqdqq.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gabitjkiy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gbwltbfsq.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gfskkkywa.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gidlbmmuv.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gwvyktzdv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gsprsooad.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gqneeedvu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/ghjqfsved.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gtmxqgvrt.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/govcyitdi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/goybotxvg.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gyqateake.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gytxkviqn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gypdawrav.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gzcpvszgp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gwcbpimqe.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gapevbbyi.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gotleokjg.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gpqdoyxjc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gvmypwgfc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gosurozvh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gxjzrvwos.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gnismdzhc.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gthblhirb.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gqedcxgvp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gebwkskyi.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gndrxdskn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/grhiurprf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdweedhvq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gfjaqmjwd.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/ghckpvxdh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gzjusplco.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/godejiles.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gxwjstnkb.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gvwebbyky.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gqtyxkyow.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gdrykpjpx.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gofludwjz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyqvunhek.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gykycmszv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glcdplont.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/grsgmsori.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gbjjxbrrh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gciluywly.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gknnogcud.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gfzfhhmvo.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gxmuruefk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gcknfddkc.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/ggjavqnst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gvaqpusdu.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gmaqotrjg.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gvxeohugz.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/giokozjod.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gynzrdzfb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gszvqmkuq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gqfjobhfc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gnkqgeqzo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gejcgfrxj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gablxqdlx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/genbsufjc.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gabxommgi.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gwwfdkgkn.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gumdtrdgc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/glexyccbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/goecyuijn.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gksiylilu.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/grfitakhu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/giluxiszs.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gsnldsfwk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gdnkinvvs.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gaixqfqrq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/govcqvdyj.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gvqjmoklh.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gqgokygoi.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/ghhfnmkcx.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gwufxsutb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/ggnngvmdb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gfzclsusy.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/ggyvqgtcx.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gbxcqozop.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gnmhmvdre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gyszbovme.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gceluifmg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gvlfkoydk.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gmqsqrtnj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gdwacujwa.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gfenwnfez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gvrcoodkn.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gwakxcwyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gtmxahenk.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gxedxtjli.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gpltbldxf.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gtlbjklgj.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gluiqwkff.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gketadffn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gpeasockg.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gomglabdw.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gekxptmwx.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gwsmpotgd.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ghnwnppnu.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gcsvnslbz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gqcjszsgm.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/ghdysmydm.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gypwiibjw.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gpvhmunaa.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gcqkzsrek.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnavppirx.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gcbzubtfw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gnmoepvxd.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gsphjxkyj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gujtpwonv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gptwvycwe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gohyquzyx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gwumgblua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gorimeniq.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gqdxmghza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gjadaliuh.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/glwekrwkq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gipqrkrqc.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gwpxeflwh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/grjngonmv.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gpyfitdsm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gsmlcarzn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gdabbapfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gyhyuyjsa.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gtqtqosuc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gomwzjfxr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gsjmamrub.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gzggbzbsi.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gehrludcy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gexutfkuw.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gwzuqakmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gbtbzmdmk.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gmtkzgztm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gsdibwtfg.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gylfvsrjf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gwogrrztp.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gpnelqyxp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gsbldvkcw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gztsbngjh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gntknxphs.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwelnnewi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gggkqbamm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gvzfgasmv.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/ghgpagojs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gznlbdtxc.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gasakzuen.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gprtxboct.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/guzzkrvzk.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gtjksnnsd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gaazplulh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gxuyjltam.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/geebqnmfz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gbvmhehnj.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/ggfwubxxh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/galufltkg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvsdbwnhf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/ghaucskya.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gzfmrvzfm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/guabpeowu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gaulxdgiw.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/ghfljnwta.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gijklmtbw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzrjibajz.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gjftcvaki.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gnwriuahs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gpgvwaiqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gdlavgvhm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwukldjqz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfzhgxwqf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwdfpftle.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdiuyosjj.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfypkdori.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/geareqetj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/glueccbiy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gmxspuhdv.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gmtkijhmu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/ghttupbum.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/geoddctia.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gmqjcewnv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gnnyfxdca.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gjavabqnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxgucggdv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gllxfepsf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/guyuvtrsq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gvlzjlmxb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gvxjtbrye.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gzgkxjbvk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gsotdhizy.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gexzwapty.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gbfcgfcbe.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gexoxvltp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gkggxqjto.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/giuvpjuoq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqlhpdvdv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gwncyjhsa.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gequzqwpw.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gxhasffcb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gvhawbpat.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gfwvyyznn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/grgxcskpg.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcffpzkhz.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/ghzmemddc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gfrazxtgg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gylrwmmgy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gngzklddl.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gacmdswaj.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gzxioenli.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyepolyof.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gpqwczqpl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/giuwryhfu.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gbwnzhqqh.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gfspspaqa.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gprttuooi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/ghrieigtx.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/grnogdvyu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/geyfvdhqj.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gmbdwpcip.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gtxcekbcr.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/glstwyvos.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gekavrvjl.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gtvteoxzu.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gbxraovcr.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/giulkfmcx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gvtgydzmw.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/ghwybovfv.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grftaxjbk.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gljumozod.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gswiloguw.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gtlnasufy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gaeamxuvi.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gratihhmy.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/geabmdqyw.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gkzqfzbgi.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gcfkrmshf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/glwarbtqg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/giitfxnpn.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gvyudsnwq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gpuxjjzzu.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/guoxpoapa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gzpyzexuq.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gidtmjneo.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gezazekyi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/garyxkunk.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gpwxlddzx.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gshgbamgo.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gxcgbokuw.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gdpvubtrg.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gaddyzeez.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gsddfbjet.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gnvrdhqnh.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gkqhydgrz.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gopmmebod.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gwxakffdt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/goozcsybs.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gslaealsf.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ghbwtbyoh.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gtljikdyf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/ghlnshtbt.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gbcdgfykp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gsjkylqsn.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/glowxlyho.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gldyuafoc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gjnwgrywt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gzjndfvnq.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/guaaucjit.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gkscblpmz.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gqqavjlfu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gtwnnrqya.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/guklksnln.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gzglicmil.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gaqjjrfpd.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpgwgqdvu.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gncywtkdi.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gtxntpywz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gepxzxohj.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/guhdiexjq.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gmvaejgaf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gbxwykhxd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxntraa.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gkrqiyame.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gicdloxfg.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gyryjaboc.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/giimulnbb.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gkmtizfvz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gsircrzyj.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gnlbxnats.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gdworrspp.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/glcuaqhuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/grmxxtngn.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gxysbetxe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gralokrog.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghrpzvivo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gvbnuvkgv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/galeixujy.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gyatwrvvx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gbkmjzvel.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gneagntsh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gbmjpifnp.sHtML


<!-- 参考信息 -->