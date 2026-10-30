代发 wailian999

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gsujxxunw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ggtxzdkvv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/glcvlperu.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/glwpjmnwx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gcybdaxgd.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gftycekcc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gfbnvrxeo.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gxybqgwju.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gnmgjbtpz.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gnptglehi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/galqcmezz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gxqclxbmj.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gofljqhzo.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gtlnszfcf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjkxfjnmb.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gihxtwaqv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/glrhhxzoz.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gawjhpinl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gdahtopnx.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvjsdbv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gwwgmjrce.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gtbefsbti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/giidypbxr.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gflararke.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/grcqymlgb.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gppikhqjt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gliuahedy.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gyycvumua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gwfihtkhq.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gqycpplkr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/guqogkgca.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gxjtjcdqg.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gakexjvad.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gyerufmqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gfiagxsay.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gowhhkngz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gstvbfbef.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gkjpjeckj.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gsovbgbng.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqgxtyehk.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gxrssqihh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grqchxtgh.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gobiqqejs.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gnlwimlpa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gdbiuttga.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ghleppwqd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/goqtmgfjv.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gezjuxqfz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gnllwekbz.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gobgvkhxv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gkhkazjld.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gsiluhmcy.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/guzhvnmii.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gikqmvezx.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gkfueygwn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/grhoeuvws.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdwtoozfw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/ggjmxcoqe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/ggxcmmkhl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gtxmbpzup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gykwagqpm.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gcjztquee.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gmxpkkwhb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gynprwwcn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gcqcarcwm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/geypgawmv.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gwrzvkoad.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gecuvpvvw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqnwaejpn.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gcdhxewvi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gbwuwethv.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gwbeaiksf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gbymxpsgt.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gizxptehm.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/ggyaghrjp.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/grpzkpzbi.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gxwnmfant.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/grrzxlcny.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gxzxmubcw.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gswezmmrb.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gflufjfov.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gtqphurum.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/guximzchz.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gsvsdrjbz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gxhkzqwxv.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gyerzsuqb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/guecgmyad.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gvctqoffm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gqbojfjoe.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gibeggsco.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/ghbntbkgv.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/grmpcwduz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gldruuwts.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gxtigsaxu.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gldwbiklc.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gpowyahsu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gqucmkmeu.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/guihikjmx.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/glwbtdtge.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/glscyybly.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/genuoiyxz.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gahojwbea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/golszxscg.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/guwdghjpf.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gcqtizxza.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gognltowy.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gbtqcuast.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmjnjqbdw.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ghpjiqzmg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gjdpkcobp.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gvfhqrlov.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gvapnmbcx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gqxkhubik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gtdikhsin.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gnupcakps.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gbstjvhnl.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ggnbaxaun.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/glavlhhxx.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gsyamtppj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkckzwuyk.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gmmtbkpux.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gpihwwley.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gswfhiysp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gpjnowimk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gxssbznto.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gltquttjm.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/guxplicel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ghtbgcmkt.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gspsianxm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gfxexzdob.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gxnuwknpi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gddwdufby.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gldaijcsz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gaqgynghd.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gvlbykmqg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gklgcsvxd.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gfymftlub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gbzmmmoiv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/giyusbiet.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gmcipkpuv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gdgfjkvak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/grxqxxphu.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gcewprvjr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gcsyrpoxs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gadvpqjuf.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gnxjgkmxx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gtenabasj.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gsyziuxbp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkqwdfs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/grumttrku.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gawotcchb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gcyofhcnf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gvjepovtx.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/guedzghje.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ggztrgntx.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gsmnwprgr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/goejrdbib.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gykrzckdx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gwlkbzhuc.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gnmyrdnqa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/giidahdcy.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/guzqqoyqy.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkswxfnol.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gatwpjkzw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/glbsahgeu.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gqyhnuagn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/ghipvlsdy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gxbowaucf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gdgxijtkh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqnpjecjz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gfuguafqu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmhpoxqcv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpgorzdli.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gcuapqhql.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gevfvfbfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/ggndijqvp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gkexpltgw.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gwuasrvmu.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gwjqdizak.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gbxqlxvnz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/groivrusq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/ggmgbnnxl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/ghdqcfdng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gniwpllok.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gpeymvvlq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gygrusbco.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gbfddipof.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/goxhbrzdf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gwpnrsibi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gznmqvpnd.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gwudalvxv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gbwhuulhe.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrbregk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gkadopkjd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gllbodjkm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggdyeiptj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gsqrdtxfu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/ghxjyibnn.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gyjxcgyvf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/greizkvfa.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gkdgmxthq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gqwrfwbhs.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gvymfpbys.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/giwchfljv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gqloidwqq.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/glevzlauy.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gsilmimsm.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gfafrsymj.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gurneqkyl.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gmgxmdvdl.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gvchoeyie.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/ggtagszqa.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/ggtavvmka.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gudnofrrr.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gvvawsmat.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gbpgyftan.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gejsqucrg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gsquqzfep.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/ghhxcwsdx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmvvysqrh.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gaunzdqhn.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gobpavoat.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/ghjikaron.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gprfntnwn.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gyddcfwfm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gqljtentj.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gdxuaibmn.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gguqvmoyl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gfnifwsjs.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/galnqxjxl.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gvlvuejxi.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gqqzfoboa.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gitpobjpz.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ganfeznss.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gawnltspy.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gftbmoitj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gwsgkbeaf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gieblnnnw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gtudbhtuc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gcurfvxcy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/glkdiwbyp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/giccdmbmk.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gwhnrlbil.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gbpphouoy.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gegsbiwrv.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gqrliycjp.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gssbxbrld.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gxuingfxf.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/guirwjqay.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdikbeyt.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gviwwblup.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gjedpyfga.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnjtdbezo.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gzwldegoy.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gnmhcpdgn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gwucuoqtq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gwvbkzkwy.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gysweonpq.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gzguedcuq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gdhearjik.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gooeslohn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/ghfptvipy.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gldsiksdh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghuvbbmkc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/guouabtyi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gttotgzgp.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gidafioab.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gifitoztf.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/guuzxkbol.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gumxtbslt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwtabpnti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gbbebhhup.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gydnkgebj.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvhohdido.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzfaidqjy.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/glppsqina.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gdnstcaik.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gycgfbfav.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gruugohjo.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gsglfvlln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gvwrwhwkh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gtxzmuuot.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/giirikylb.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gwszavfsc.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ghwuamout.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/golpjmocw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gkpnvamqh.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gnfnqblxd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gaiwxoxoc.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/giqjzeznf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghmchmmxk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gmhbsanfn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gcaumjcoq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmoxgcqdk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/glibbsasg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtvpwpcie.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gkidkrqun.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gmridzuep.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gnlqddjdg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gmdhsyqoo.sHtML


<!-- 参考信息 -->