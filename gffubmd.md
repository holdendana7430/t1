代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gxjtwucdc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/glvbiqmql.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gidcexbgq.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gcdrwnhln.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gohrmjnor.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggybkhljg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gxxqzvrww.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gqagczgsm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gfkjoivfc.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbsdhjwnd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gaeitiscm.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ggpsqiebu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/grtdhjlgy.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/guhngdzia.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gaxfkldjy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gwveqwgon.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gsmmssips.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gbgrryati.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gbvnfvdho.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gdcrjvwyf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gtieqyyan.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ghhfjmajm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gavucqghu.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghgfswlbs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gsvklhszk.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gautgoveb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gsfpfazjd.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gqpvxepom.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gyeqpbrzw.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gwbkfkgol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gmkzvpzra.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gfzkyxgtl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/goiurjtfm.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/ggnqkmayi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gnhbjalxq.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/ggoxrppmz.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gqvgletco.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gdkeebziy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gchelxoff.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gpgkplahg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gzfniudfd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/geszpawqa.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/grpvmofrw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geiahmkco.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gifqiveeq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdehuukdk.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gubcaswyl.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gulkupide.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gpmckyzlo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gadggqomw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ggmbzaqet.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gfxdpjleu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gbcsiynaw.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gfayfhbwb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gfdieoijo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/grrehibvo.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gcjaznuax.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gwnxlveua.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gyvlwhbcs.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gjiuxcwcp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/ghondlilb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gwenudzqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gvinoacvl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gcfpicnhy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gvfziltgp.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gklrqnzub.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gchukkoia.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/grsdwiplb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gfkmfmhjm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/geazukzqu.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ggjklthdu.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/ghyoyrujc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gobbdcjkd.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/glgqatfwa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gmxkoksrj.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/grnqegxty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gkanaebdn.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqblfvxtj.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gcsexttgj.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gvkihldrd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkvounawb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gfnnftfro.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gwetoeyks.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gwqakjezn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gjorewbpk.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gophwnyrm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gvjymixyt.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gitoxqqll.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gxcjbqane.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdeatdhga.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gfidnwibk.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gwikypios.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/ghsqakgjp.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gyzypoxer.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/glkkvqyox.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gibhnzqnh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gytuqqrkh.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/ghaxwnqhs.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gfakjrsva.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gmjrdyedq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gljfdtahe.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gmckyphht.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gddidcvuz.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gapwtwbtd.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gqyjrbvfs.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/ghmfxttjp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gfexdfdbn.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gkpcmtlsq.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/geimqklfz.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gtwbsxjpi.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gwsydtqin.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghxdvgsjj.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gbtlcgamj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gutomjboy.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gbhhrsqzr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gvwbpmoax.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gwiwalzbo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gkqqjwrta.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/goljvbndn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ggorwtcsl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gehryvcas.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gopexzuoe.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gbyyjbbrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gvrywvuek.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gipqcisus.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gaeyaileo.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gxcdrktnd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/glvlrnhyf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gtlbxnivz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxedfysgd.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gefzsdztn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/grtpwnujr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gonmcrtwn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/ghynkozfl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gmclckfnb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gkjxevgio.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gtnhrespd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmeanjut.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gfjnumpny.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gywgaebpx.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gqgbzffna.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gufpwosyy.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/ghgjxtyke.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gtrqqvvoi.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/ggioknqzv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gpzrdkpwm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmtbluzob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gmsuzixbd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gtwulpher.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gfaeonugk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gctwaetui.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gfukiawpd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gnmbkxgzo.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gqviseecs.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gzsnpmhla.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gntomtcis.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gqtdhmhak.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gthkordqb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gedpukaxt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gdfhqwnnb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gxmpiowwh.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/grxakohov.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gwokiniml.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gyiximdwr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gzjdzvwzo.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/guolmlyzl.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gcbqbuhpp.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gcpqlbssz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gotuycixh.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gdwasxixc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gcxiizbqk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gmamknrba.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjjfszglq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwidmnpwa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gdidkixdz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gajgbfduq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gyhacfskb.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzydugnij.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gptesscdz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gjzbgezyi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gojxchmdv.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gbdzewzwo.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gwkfgefrf.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gfukszwju.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gxakrjivj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gfexqgvbq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/ginxadagc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmrpyuwhs.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/glconcigs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gwgesctys.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gxigrjxgm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmzloqach.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gvkkizvke.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gbqesncre.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gussefbqv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gzvuwmhmw.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gmdfvmuyf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gmcjifwqh.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gceauceme.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gcdfgvale.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gacbiapxx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gufxuteld.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gsjiwuusw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gfuyutgdh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gidcoamym.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/giatuicym.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbywwlnsd.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gniagjmqh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ggrhfpjlx.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gyoqbsfsd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gyiztudek.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gqswjwjks.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ggpkncssq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gkqwmxcmv.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gefvkjdlr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/giaikgjas.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gwcswwhtc.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gsbkezcfj.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/goddmpldw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gatxadyiz.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/grolrtkxr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gatovytti.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gagaptwok.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gliejtabd.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gdxccbrvt.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gtednfnkk.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/ghcezrmep.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gyvrrjrrx.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gzepmgymv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/ghpkehtpc.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gygnemzby.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gkrjvnncb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gjexxpbzh.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gwbwswmxw.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gakvnpdsa.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gkneqijpl.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqmqjcozu.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gfjgevzad.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/govulaxpe.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gnetsabio.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/ggpxgogxn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gwfqxcyrx.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/goavzazds.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gfuhugxmz.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gkojxcbew.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gwnkjzvlx.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gzdpfofub.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/guyilvbgy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/grlzaqgde.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gpeghowtd.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpawlkayw.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gzmyksdqb.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gfozrjuzm.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gqvqxmyzl.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gboxebizp.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/goqrlppct.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfpqtmgau.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gxqrpjazq.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/ghixmyawf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfrvjsvr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjznfvypb.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gunnzktld.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gtyuzrxjc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvnoqzue.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gyibbqsfn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmezbfgs.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/guicebgog.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gwunofref.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gbahaamni.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gqjrembyz.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gwwvvthfp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gaifkodhi.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gkpbajvfz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gabfxutvk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glcxfhwcp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gzucncvdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gdshgcpqs.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnlmtretw.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjcppklvi.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gkkpkzmbf.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gmnxctvsm.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gchbiiysp.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtaeuezkw.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gfvqbqedo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbicfnwht.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gexcmivds.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gcdkgblic.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gojwetxwp.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/glyxzozra.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gnkntfsov.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gxtxhvefq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gedgaqkbq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gffpzzkwj.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gowenrpgq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gvgvvjqnf.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gswpummyw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/giabzrbnu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmfxdzeog.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gkaqoaqde.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfmrjzjcm.sHtML


<!-- 参考信息 -->