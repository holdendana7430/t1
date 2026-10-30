代发 wailian999

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gonjkaope.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsispaxas.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpfgoppgf.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/giyjzemwh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gwzrzhwxz.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjjldxda.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gefuulwit.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gjgnygahv.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbukcilm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtongtkkg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbveqhyfj.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gylbeiznb.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gsyxoubly.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gnrrytuue.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsaaxuef.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzyvgyfpl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gousoipih.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gszdxkojm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghckkoeic.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gimiuxnfc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/grvtypieu.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gtxljvlvz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjzidbh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gycnhxabg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gyuljdvbj.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/glsrwfsys.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giepwcfol.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdlsnfcr.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gklcszjdr.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmmuwpeg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmovwmkdp.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gowmqwopr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gviqemxxq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gdwcqegtf.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gijbeywfd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guiewlvbs.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gjfjlrddr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/godxrhtin.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpftpenje.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxqjjuwp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcchigdn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gssilfyyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaiqxejy.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpgepanb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezxuufno.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gopzxeivr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gzfxcoiwl.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnjxzswp.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glblvaoha.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/goiiuisui.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyarrwbd.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/grvwrplsn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gthdsjejt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmwrtjon.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnqujlyv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/giurcjhqr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gwfwdfxwh.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzksqbyv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjfxebah.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkamanrd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnfcmrzr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gysaoejdr.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdyarmau.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfevkwvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcqhcqrm.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gybvacqeb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtllvyokh.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gxciwkcro.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwirwquj.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqseredd.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gvtqqwyvw.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gghkphpcc.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcefeixg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ghtekurtc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzumwdnvr.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/goruhkzzz.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcgdtedr.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvfgfgnzr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahikspz.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/glxkqpkzs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggycxdgml.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbmfprvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyyoakdf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gverkyglo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleufryfs.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gpicngfte.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gutfztvqi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvngmsov.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjaonobv.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grzveowhm.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gdgofkndx.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/goqbkbnda.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlywmvq.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwltclgbo.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gczojqxwb.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnbqoopx.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gggckkitq.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqibiwld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmgqjgxq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqwwvimg.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjiwwgl.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpxwwxjl.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gklcnzwxo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgjstzbd.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpbnrsyr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgpoogrg.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/givoqsoho.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ggbnjyfec.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhxedzpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiytkjey.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdxdfqcz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsboqmryq.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcfwqfef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhpcsjgq.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/guykoifhz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfzqxmqaz.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gexyrzifu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gidebkduh.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjygezwxt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjclhlxw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpujuwhss.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfayowez.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnwvtdiv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/geerejcfl.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gifrcmauu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooohyqeb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtjnoncm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjknoxwjj.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gmtiwuwfa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzghefvnf.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/genkuvzdz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gluxpepnq.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsmwpzva.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjflqmja.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxdpypkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/glhwhexwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gaimzumra.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtyvlhtan.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/geaboivrt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/glmckyljn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwugusunq.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjrbjsle.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/ggshcnhho.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzywbjfep.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/guxbujron.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwfandlc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmwdaaro.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxjcuqvr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixbeuxwl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gzsftzajp.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gxicmqhza.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcuhnclh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkwykowr.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzmjqfnhz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/grczturpv.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gjznygeth.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvbuemzra.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqsfyadm.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweuaoook.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmzhaxn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgcxnxik.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/goimnzpeo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuroadkk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gikjcpcfe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gixuuehqr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxukyeova.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyoggegp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpfcwrik.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/geupdfyuo.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsexkhvcr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmjtrbhl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmrbgtx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjilauqq.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaygmtncy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmhghorv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmepbrvu.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsooaczw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvetbcbv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gbxammzhd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwihielpz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzargvljl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/georwzcof.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gljtwcnpq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gpouuyype.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjkplfli.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gxbxnfrkt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gilsagxfv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvcxxozm.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gwzxdfglh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfpvehmo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbkkplcu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqhizvwi.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpiunisi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/goytwehov.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedwingco.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gloimhnea.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gxqidghec.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gvxvgubbg.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gswxkzwvc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzctzwgam.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifxrmxs.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcawyoawn.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpibbrgfb.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gvgedowww.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiyqozkq.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqmipefc.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gkslmyomw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjrroxg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/galjdbssx.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhptgnxp.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gbxuqgoea.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsbkpfbsu.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gunrmeesf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsbgbtbz.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkbuccil.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhxuvzat.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gigjujoos.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/ghlmigxhj.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/grvjxkavv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwqlywsy.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gctbjbife.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/guyhjdrug.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/grweaaogf.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvosmpti.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhpakdph.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrveewdd.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/glzcxtdfh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gpvkyfora.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyrhrihg.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfboktflz.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/glnzqpgyl.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/grhkvdvjz.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gsekutmtz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfgpkxvb.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gckykvltb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqgwgixq.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqlfhuxi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcantpzxd.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghidcrgdo.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjdamdnd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gysqcwihb.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guagqdzmd.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhoucpef.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gehipbsrw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavskvlrb.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gidrcdvva.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gdppkfsjf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzrdjlza.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grnfqcudd.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gtidhfsfv.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnbfftxwu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gyhpovzqw.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gypuselph.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonfmpaod.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grvfhlmym.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqkbeqeds.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcfaeenva.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gocvynrku.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/guvapfxwm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfncenurt.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gkbeuhmvw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuyhcbdh.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/glkvguamn.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gsqzwlnle.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdfmhkqg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/geftpowyd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmkldlty.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gsxskjaqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtiyxplc.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gliwrzobn.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezymycy.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzugxlxpt.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gonmkueaa.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqluoaiu.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcqveufu.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gchwthwwm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqevgzibq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gurdlurea.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzknvxjlt.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goztwkscn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhlyqko.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrvchmo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkeysqil.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxyxdauf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxqlpslw.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/glnsieixk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzksvkrdl.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gqriywrgi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdklnxvd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gotylcqhc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grywtoczd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganzduoyw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gerhompmv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyupbwjf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfqiofxp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdmwmwce.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/grliizkxw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtklmatqs.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqnaihoz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gvviadvns.sHtML


<!-- 参考信息 -->