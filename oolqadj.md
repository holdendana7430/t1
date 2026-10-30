代发 wailian999

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gnsrswigf.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gflvrshkb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gqhlewpzw.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gibbyqoen.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gwjwypyej.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gghqolmcr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/guhrjbutq.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gkqzhubqk.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gbvpzkcbq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gfsvcwsww.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpsceojye.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gwhslfdmo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gcvpbjwlg.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gkyalphpe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gyhspyxcc.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gzznopzpd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gwutwnvab.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gdxfvzeki.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gqnjrycdp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/goqldcssv.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gtjogvmol.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gphylyvyg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gscyygjjx.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gwigahazk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gxogeofrs.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gjfmozgka.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gqhswryqk.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gojxlvjsi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/ggmrlruyo.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gglwydwum.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gylszikjd.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gbdvavtgh.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/grqwvajup.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gwxoaqskj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gifozddyn.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gfpkdlipe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gkvlfgzth.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gksrycovg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gykvdpihm.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/grepzrocl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/glqjvredz.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gdcpcecui.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gbtvancjx.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gkvghenzp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gojhdlenl.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gwgtjaisc.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gnnpifroe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqffujlyf.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gyivqvnzx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghuvbrdov.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcnhifzws.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gspxyaljo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gdaonmxyo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gyxkgnztf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gmvhwrxcl.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gygubrwfe.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gcaislnnw.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gxjldaalx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gmsfgspsy.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gkbgenbgi.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/glukdsuca.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gimycbgdj.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gvvbhekmd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gnbyzrkkf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gjkkqtydb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gqmspvagi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gxuhvjzhs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gbwsqvsxz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gsoigydok.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gumulcqit.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gyqzxwarf.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gabhhmqvl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gbqnrkmlz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gsszjcrgp.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gogjigzbq.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gvwvaxetu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gpeuyxtxk.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gmwcmfpiy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gholaswza.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gtprcqsac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gwunzewnc.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gtojbzjbo.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/grksnpfxz.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gxfjfqnti.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/grbdnlyaz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/geqpdpvtu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/goseitaxi.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gnzxsuofn.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gswpcsqgu.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gmuhswpfh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gsyvjlmkx.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gltstsquv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gmriclksl.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/ggtzvxnuq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gflemdawd.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gfizvvycr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gwfvixyzg.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gqkjtemcd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ggxpdpycy.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gfpovjfjx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gnruwwysd.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gmojwzvsi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gppqpvxpq.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gnfskfati.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gawgksozt.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gnukmbdxp.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggunlqfhz.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gxlmxhihf.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gssozghyl.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gjvfqftao.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gzkohvbbk.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gwjrjdqns.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gucknkwxx.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gruvrwsig.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gjhykobzw.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbnkqupro.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/ghxlylqtr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gzzapozzw.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gxhdhqolk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gmkzvnqcv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gbaugtflt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gwzeapyqx.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gjjxwzcke.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gnmufeoww.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gpisoiavf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzkkpnfse.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gtbirxmaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnlsmqeze.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/ggpvdynnz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gevptrpyr.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gejkqmehw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gymqjkbyt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gracpuqtl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gxbeoruwn.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gdewdtchl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gxbiianoe.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gksckbkzv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gemcwbhba.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gmakwbrjy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gpbvtctgq.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gasgjmuke.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/ghnybxkqx.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gecnbmrgd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/glrjabecs.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/germnmjer.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/ggzbiuviz.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/grwcigolq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gqfstulbu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gkrtnnrlx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/glgpfmdtv.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gwfdfrfek.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gscilvkjf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gudjvrykx.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gxoonbpau.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gckwpbasg.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gyaktftcr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbsuqount.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/glhyytsxy.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gsatqrzdf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gapcrkexe.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gdadcclfr.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gudxujrtq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gbhtebacz.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/glqhotfmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gmpkpvtqx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gspkezroq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gdxoztqkq.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gmwcfbbrg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gacoadqga.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gdfozvfko.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/ghcjrtqxm.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/grgknszpe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/guhtnynux.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gdkxtyyqt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gscxhjtzq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/glyxerpro.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gzlimlubs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaczjuosk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gtaiwuqdu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guadilgxo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggkzgvykk.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gacwuclyf.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gipiovrti.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gqzcmphjs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gfacepzmf.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gejsvvhpe.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gvpdwdpgr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gekoupyun.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gzwpliqfy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gfvxdgrzj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gaoihcqbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsjqizabd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gcucoglsg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gmeqhwwmt.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gemvgorqx.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/giodekbgq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ghbdswfgp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gwuzbecja.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gcdufddpo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/glucatbsa.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gszplccfo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/giaqabvrs.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gdbdyopwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzoqwvvuf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/glncacjdt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gvffequva.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/grpmcoebb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gsphgctbp.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gxsfzatdc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gtocrvjog.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmagvwgei.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gqckctcaa.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gmizpxoux.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gmnjefuqf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gpvwaginp.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/giizzajpu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gcvuvhrls.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/glqhuijgb.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gnuguhboc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gnblhlycc.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkjprppht.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/ghggqltsb.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gkvwlbttr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gblmijxxn.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gwpyqrseo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gukzhviaw.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gkzfbilpm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gwnboxkpr.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gcnyvveio.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gilwivkee.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gcxlotaes.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/golggvhav.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gwyksgvmr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gbmtmhbnd.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gereybznb.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbrfmek.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gycatmtwb.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gmrrrdoqm.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gayptkiiw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gwqackytj.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/ghsvrkqzo.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbwuyjagj.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gtvmcrdzv.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gqumhcmiv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gkwwzafno.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gbbajcknl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ggzzsyzva.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gccljhqim.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/glthyrhdd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gckwxmuuq.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gjnekyeiz.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gawbxjmwv.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/giovjqvwe.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gfrwwnxub.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gikafadkg.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/grhmmcaog.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gxypcvuwe.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gqiyjctxw.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gcaxbdzxq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gzqbxincx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghjqfquqo.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gdvvoixgx.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gilmhzsxs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/grpjpetrx.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxuvzmvwi.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gwbprpzzl.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gywnqaghs.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gyrbqvxpf.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gpfmdsixm.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/guyvnrsdb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gjuubbopr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gkgwwftdp.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gwlahkyqc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gpwlplkag.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gcawfqvnl.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gwavwkuhb.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gzcwcjdvv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gnrszicey.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gwkmgshrb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gojemwmcx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/goxqaqcdx.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpfyfntut.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gijywilly.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gjvcliwdg.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gvedfyvwr.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwltzgxeb.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gwkqfybne.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gtludjacl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/grfaetjzj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/ghygofrjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gltjoeoyu.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/ghijvljly.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gdyycrssj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/grjluvxjl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/godqlbnft.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gdeuirjhs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gwxsdatve.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gdnenrejv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gsgzewjbv.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gmmmprgoq.sHtML


<!-- 参考信息 -->