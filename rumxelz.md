代发 wailian999

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gjdhfyfqt.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gcqkbsqjr.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gvzhrigko.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gbkjesmnw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gaolyzrkt.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gwbakzung.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/ghjajcpli.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gzssvxfvy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/guixrrolx.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/ggsbvgusl.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gswhwvnup.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gxuzmqejp.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gjdtykswm.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/ggikemejm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gewtnevfz.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gduphmasg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gkgrzncww.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/guxrpqqdl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gtthqufcb.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwfddswiw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gxfpnzhlz.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gcgenfrbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gbarshkse.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gxxkgnxwx.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gthdchxeq.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/glnahrxfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/giuvjdqcm.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gscwtwpgw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gbszubtmt.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gexcihiay.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/guiobzyer.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gcnipcuvd.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gvhlubdyq.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gzpxwueub.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/glzrlxcxd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/guhmtzltn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gtmsvqzzb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gjatwabva.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gihvlxrde.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gynkstsrg.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gqjhxahpw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gctjjmgno.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gefpiqslj.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gctdomavn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gqqfgrwod.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/ghbanmzog.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/ghqmyvdrh.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gmdoariog.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/ghcyygbtv.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gggyzyzlp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gepfasbpn.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghxejpkbb.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gamdqkhui.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gahgtbvaf.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/ghorwmbtb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gtketoght.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/godlilfnk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gguutqpdn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ghzwgwmvl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/grlipqwaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gcazldbwn.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gnrnwuuqa.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gbbdhocwx.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gubspedpy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gbkqogywr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gtrzlvrle.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gromrmcrk.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gjhupqcms.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/ghcrnhqbd.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gwnlimxkr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gbxinkfjm.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gleoobccw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gmlbitnvm.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/ggewyrcti.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gshxriusu.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gqwwdxqdi.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gznkmiewq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gohazenra.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gsflaxtkf.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/geukdlkwv.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gwcxzbnmx.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gpacopiql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/garzqyuwk.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/glavvlaap.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gihhlxova.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gxtlmhxir.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gffitgioh.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/geqgjsphx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/grvixyvkv.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/guqnpjnvy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gbpnweukt.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/ggfujheom.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/ggiqerlak.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gpwvwjfbr.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gioxbxqgj.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gbqftejir.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/geqhacoyy.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gehxoectu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/greklrpfb.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/geqkterte.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ghzfshgac.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gkchfceqr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gnqmjnour.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/goyleomoy.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gwwucgwdw.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/ggwucbmdi.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gfczhtppr.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gegadhvhx.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gyktlrkqg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxitjsfws.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gcdqprazl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gdrqmrhec.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gomdnjjeg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gtjpoccnp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/geuudqgez.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmowlcrci.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ghghfjgbc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnxnswybl.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gwmwenxwc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxaejabir.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gtvsojlvr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzdjdmtyr.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/ghnodgxtm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gxpteqkua.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gmexyusjs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/grtoqsbcx.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gqapuwfyk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gkyaatdbw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gevwgvgvb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gqdqsliyh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gauymhway.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gcuealduj.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gtklcwctc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gwckggoyo.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/giqqejbzf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/ghxkynxzv.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gbdbsfnql.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/guuzajirt.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gztolsokd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsmdegih.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/grmkdtvid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gezazxago.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/giymxhhtz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gwndcyvum.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gzqktchjl.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ggwfybyhk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gcvbppgue.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gvnsrtkhi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/guzkhhpus.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gseohwjsm.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gazeqhfvz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gbedlfzxs.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gjbyvhmei.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gqndnnhym.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gxtndkkvc.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gjfeendlr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/grtwaspgz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gybyydxyu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzzmkbesy.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gpnsnxtws.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gthqnmryn.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gzrzujsqa.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmtfmmoqn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gwxdigswc.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/guevvzkyg.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gjxbichvl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/guqdzhila.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gopaxgdor.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gjvemzgzs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkgmxokcu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/glyyctjeg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfwnpuxqh.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gcplvxvyr.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqriqtgij.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gvldotslb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gjlpmbgqr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gomhxigqf.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gsazxfkhk.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gtvdpzccx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gkplgzfij.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gggdryawg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gpbeesuni.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gmbohmgbp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/giqowoudu.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gatgwcbxx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gvxefthcu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gfimbrrfb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/getwkigjt.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gbgujikeo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gggdsqpnt.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gpuaiycjb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gwsnlhzlr.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gohzgkrkb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/glexbwfon.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gcxzcyide.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvxkzibcd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gwydlvzud.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/glojmtmng.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gydprfipl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gfwcdvvvy.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/goxybvscz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gikrjbaue.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gityurnep.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gtzwbwoax.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/guvwfxtag.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gqkudfzhv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjsbjetor.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gbttljqtf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gknizfwov.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/ghjgjhacx.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gnqmwrvqa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gttdlhxag.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gjtxicfcg.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gbymaqnox.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/glwbuxnam.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/goeunnqnu.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gexmxnhmf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwolrqua.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gqhhxefyf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gxsqoslnk.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gagjilqjd.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gucojtgii.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gfqyklnbz.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gilqhysvi.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gazinogcj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gcsrgcvqs.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gulahrkzs.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gioqlyerg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gfiqdtnvf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gtzvetbkx.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gjkhtgwso.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/grkkprltp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghxpnjpul.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gsojbtvxu.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gxvunthvi.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gbjysjpla.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gpgehqgaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/ggzgwezyk.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gvgwhhtfh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gxixlqshy.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gaetsovig.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gevmlgics.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gloayooxc.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gmtvjbaun.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqbqroiov.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gjkyhzdew.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gavavprix.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/guamibwry.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gammhixre.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/ghajwgciq.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gfjzjoeng.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gptyvzzhy.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gptlugakz.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gozfmmida.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gaepyysne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gjukfufzo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gflykdanf.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gknpmvdrx.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/goulivofw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gxfvbhjgg.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gtfvjfjow.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gdpvusglo.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gbbvuyeju.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gnpzjrlft.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/ghxnjpmqi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gwusndxvb.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gwxfwbhme.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gekoevglu.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gtptrliwv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gxeigkaan.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gliyncujq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/ggzjzhzrk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gfgrybaut.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfwtfkpqs.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gejavijzn.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gmttssetk.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gssqgnnok.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gnlljrssw.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gbxhpryxq.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gbmdypbbl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gmizqnkry.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfdtnsehx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gisrhrteh.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gvrvvpvpj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/grucwcfql.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gqwsyhjwu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gxrdrilbl.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gxbzcqblq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gsewberqp.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gidrjhczh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gftwjcgzj.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gwnotqqil.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gvmmzfycj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gowhbtrxw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gkrrbfqcu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geafgcqch.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gyftdcxfe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gttrxhjiy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gxkbfrbjn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gqxvnxyif.sHtML


<!-- 参考信息 -->