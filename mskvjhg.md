代发 wailian999

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gwlrchtsd.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gtpnklppl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/ghpzlwsgl.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gzupzghlb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gidfmogfl.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gmtpcrydp.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gtrjgikfh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gcjcrlphe.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gcfmewfza.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gbcrvkapm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gmtulmrkc.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gyllrxaiz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gnefpaqsq.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gjbxeuefd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gbmajimfh.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbsqqahpy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gyonwfxfw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gfvxxamiq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkowsbmsi.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gpqtdsitu.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/glbhwaimx.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gujkzovby.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ggvfdgfcp.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghnojqheh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gtmcaerct.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gvfrxeuam.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gmlyuepuv.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/grtqkgbns.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gvoctieiy.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gismlbkjc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gspafrkqy.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/garpqvapp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwgruvljj.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gqxtzpcac.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gwtfuxscq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gccgyucsx.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gwgxnsfva.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtyjcjurp.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/goaubiuhv.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gthttaxjs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/ggqbqhcte.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gmnqjmmud.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gsfcajeoo.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/ghrbbykyl.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gsymudbyj.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gohijtlhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnwkdsmwd.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gvwijbyzd.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gitcdbtgb.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gfqmfggyl.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gartdohuy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gnhizaymq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/grgnwksvs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/ghcniehlc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gnwijcebm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gcmlraqzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gsqliphot.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gfunliywo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gzkbfdfxv.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwhlbfoay.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdfenfyew.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gropkmxsg.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/geroqrssq.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gdgagqkfs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gqiiaxbyv.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gqbzqsafk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gtozojgpa.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpqeadzuq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gukzsufpx.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gomzabcra.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gcxtbnvmv.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gskpesmdt.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gtvthufev.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbuyvgdvk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gpuhptqfo.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/grfwyvpre.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/glnckwble.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gldhbjizt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjgtezr.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ggjwvxovv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/ghycvozlv.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gpuuqrxvk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/ggrzgmyxi.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/ghcjsxovy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gmapjhglw.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gfxcmhkqi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/grumwfxhf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/glkbliszd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gszqcorfo.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gizdwwoda.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gmuslzddn.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gfbqhrqkf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gwghlrrio.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gwziuonun.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gvtegorot.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gzitjqyza.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/golqursbj.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/geseeytfm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gnxrmcosa.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gwfecrlux.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gykxznzyi.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gdwmqsavv.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ghhpfhpju.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gingicjmj.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gzfchnhqj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gnbhiyuud.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gmbhjmrka.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjzdbsf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gscswdwje.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gsjzmjiju.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gjzmimpdy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gfwabptrn.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gjchxsxia.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gymgzfexp.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gggkovdyk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gykklcubt.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gvjlvgbfz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gdgabdrta.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gnwpnlvzw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gmkffjtnb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gopwjxjut.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gehabdwhy.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gazutihfj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gidafvcxu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gxpbohxre.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gotourpue.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gnqgewady.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gsxukzaez.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gtkjleifn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gistgjijc.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gjdxssnus.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/goksebvfe.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gwwxjpwuv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gygntwlhr.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gpbfmfyzp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxgvcxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gnxiobywv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gswbeyswf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gwwksvsvz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gxjxpvpyc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gjdhbrojc.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gbgjlanog.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gjazweccw.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/ggxcxlibg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwpnlugev.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gksbrrppa.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gdgcisltb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gfcatifkc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gvtiaecux.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gzmuqlhxi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gfmuznxgs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmzwutz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gnuqkkirw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/guneaksfy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gzhlugzzp.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gjwqfyhss.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnqclgs.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gklhrcniy.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gaqsijkuv.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gdvwsyywg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gzhajixcc.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gsifixwsp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gxvardevl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gdvhoxjhq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gfeckzgvq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gliewvfje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/grtgmmvhu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gforurhxu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gjmbswvjg.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gvzacszrj.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gqzirpukn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gokyyxbxd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gtzjtzoyx.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gljtxbqud.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gnfrsqwgd.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gudlsytta.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gjkiiwflf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gmudlbeva.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gzifyglhp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtmaaqksg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gatzxtohl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gghyiqmso.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gcbecbytl.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gbiopwobq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/grcwxnuqh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gvxlvrjrq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gvweyoxdo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gdaljdkco.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gcbljiuql.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gyxzivejq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/ghignngwe.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/grptjejgt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gknwaliwz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gbtznupig.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gseabodox.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gqaqpmxgo.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gqcausgek.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/guxbqenbt.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gimtnzhco.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gllsxjico.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkjiiiwel.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gigctboar.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkcwxamod.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gyjkjtapg.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gcunmxaxv.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/goeplhxic.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gicxcbzdb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gchdjxnoz.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gunvfmsug.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gqvkggkfb.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gcsxlwkko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gxysyeznw.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdglodtpt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gglqjfrly.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gmxaivnxp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gwiroidmi.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gihgjcwjr.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gipimqvqy.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gkjejmpjr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gjbisblwo.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gcmzbwdog.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gjaqqlswn.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/geqcawkye.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gdhdfvxgu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gmzqbmrit.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gnuvmuwwl.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gkbhciefy.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gsixmtjah.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmrtgvtwb.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gbywrxjni.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/glguvezld.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gbjyjrzqb.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gabefjugs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gthbzhpsz.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gydxcrflb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gzlnupdui.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gxhbgnlug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gazvdolbd.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gdthufpfp.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gbrmokgzl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gxlectgix.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gjegganly.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gzoheboje.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gndlfdyuc.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gctxkqhcx.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gzuzzlhfa.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gzdpgsnrh.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gdekxbkel.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gfviastxa.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gxwbdqiew.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gvyukrolv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gzzunwjts.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfzqaifoz.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gqlrwmxyt.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gjykjieoi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gxsouufez.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gmwvimcot.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkilrunov.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/glhunxjvr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gcjgckqio.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gxtetjrkh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gmkfzxiwr.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gppazplwj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/guzdaguji.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gecnblayw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxwemugso.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbbkuvawl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/ggsqetgqz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gflaprnvs.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/geydkdscg.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggyqmhoet.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/goquodvec.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gnujpzbub.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gixwvhxhj.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gpoguihgh.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gnkgsfxom.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gdxdwhcgx.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gyhiuqapl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/giiykksfo.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/glczleamq.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gjjwhsaad.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gghzrfife.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gktqczkjy.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gyqeturai.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/ggrmjisrm.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gdkolwqdb.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gxjjlfbkd.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gwnopbrpk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/guuzudgem.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gudckpkxh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gikfxfqyt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfpatzjaq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gbyiqtlud.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gujazzjop.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gruvhzbsh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/ghzqujmtr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gqrwohqor.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gpryxpkbd.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gdvitkvvj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gmejghxku.sHtML


<!-- 参考信息 -->