代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gecieedqg.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gmsffxtae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/glhmwyqqh.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ginbncntv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gwxbngbob.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/ghbjdzgdx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gesityxrk.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gnhmcjgtp.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gxqdkzfys.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gragahsrw.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gyliclear.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gpteizqtu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gpqfvozou.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gclorplyx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/ggxjlqump.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gompxycpg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gdocpegau.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gfuwgdzyr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkyrguu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/giolbqmay.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gbjyekbsd.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/ggfcsdkhq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/giygmruxq.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gqiqblyuu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gmoxdcfij.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/goiscrvyp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gatblhdmp.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggvfuomig.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gtzhnsaeu.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/grlmqdofh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gqzhoeebn.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gtcjlvhhn.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gxlnnbocs.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gwubjoizr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gcmadjadg.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/govjaygpy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gyrhxswlt.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gvxtuovmz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmwtwxuqk.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gumceeezi.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/ggsjmfojc.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/giwkawuyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/glfhrrehx.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gjtogmqzd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gnznnflmz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gphwnlbjw.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gnsaexnuv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxyczczqn.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gwjxfuqav.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glxvwkcux.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbpatuqtg.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gdhuksxbl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gzjridlsb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gbzngxmzk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/grrtwvyvb.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/grwljkewg.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gduqpnoeq.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/ggxvilhyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/guumdizrc.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gzggvmqdr.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gddswhawd.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gsgbnqahx.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/geaqphzuz.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gdiohnxcw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gvrqxgugb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gdtufkynu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gxonijvvs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gmcvzbfym.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gypbmgokj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gdzcmqmqd.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gccjjmzju.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gentkcnee.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/goynzrmvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gxkgdylwl.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gdoagmyjb.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gnwounmet.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfaqzjtbj.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gdcwkszfl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gkmfrwmag.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gmduumdph.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gqsstcald.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/ghqbxnyvj.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gzzebkgyg.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/ggaxbydub.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmjocmyj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/grorhmzqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gyqgtdlgr.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/ghleuaowe.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gffetmqwb.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gacyxtfek.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gjivnazhy.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gdlfatcvu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggvxysgwt.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/ggdhxqydz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gskvmqguu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gexcarkqn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/guxrhnlem.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/grqxpksgv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gblfvrwna.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gyhcrhlta.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/grweboxjm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlylzpi.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/godnygnio.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/ggoxlmhkm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gojouxses.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gadfifllg.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmlzzpgpg.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gcrffainz.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gesaxxalk.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gppxqgpbd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gehkjughe.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gljxwkepo.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/grlgnbhik.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gflqvyatd.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gpzvzinuq.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gxthkqceo.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gysfstpex.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gvhubohxb.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gxyeopeto.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gcknxruqs.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/glwmfsjgz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gpojvkqdb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gfnqfjima.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gfosavszq.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gjizyvwxm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggzgvvvct.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gayccxggy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvophgqqk.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gtmiutdxw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/goabrykya.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gbpnyfvud.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gnpojgemb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggyazkceb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gdahsbggl.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gwqvjvgsp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gbmfxsyrh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggxmvfkum.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gkrydqjpa.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdaumbizw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gxsgqdjah.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gfktybpzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gvfqefiko.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gguywdfdp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gqeuwsnxq.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gszcsfemg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/grgybulnx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gehadthym.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gnnwdpvvc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gdvgnncno.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gpsqjmdcr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gqjfsgpdm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gxwjiqpws.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gxzqqgwnm.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/guqrpajka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gccjjdwjz.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gtdawfzmh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwwvqkhtl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gftthrbsf.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gyntummay.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/giraxddkf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/geqjvxglw.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gmdxnywsv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/ghuzuaqic.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/geqpljajj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/garcpfwfz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/ghsyupezs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gunkjxwgl.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gzgwesmtr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/ghgdskgrz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbhxzvh.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gfbsekdbz.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gqtcdsyzq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gevohnkwu.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gwikcminx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gldbwzvfv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/goadwvoqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdidtcotq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ginmpmomf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gagwywqjj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpaiatvhj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdrayhynz.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gnuapkzcd.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gbsabbcyj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gzpuaezda.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gtypraowp.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gqaybzsnm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gizhvtlvy.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gnhtcdqgn.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gntoyxlfo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/ggnsaciqx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gpabwamik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gotgwbcqn.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gwtqqeswj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gspaldmos.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/guewvvxld.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/ggqgudyfw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gcecahntk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gpquwhgpq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gshzsntwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gmewgkhxl.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gtswyrhue.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/grqjitluf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/grlxtbngn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/guimnukby.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gjtizyqwd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/ghgbheiuw.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gctzfvcag.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/geyyyovgt.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gqwhqczuy.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/grnajnmcd.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gnroeskdm.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvdjihcqe.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gulznvqsb.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gppigtktk.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gyeryyizq.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gnfuegcqy.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gixpkixxo.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/grldurrpo.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gioadvcml.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/glsnhzvkz.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gceczptgh.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/getcnxfaw.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gcoyvscic.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gxhcwuejp.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gmetznmop.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gzvttqhws.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ginvfjnfa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/grtqslmuh.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gscysgksm.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/grqgkebbt.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gdjmywgww.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gsikdkcwp.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/geuggzojx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/ghmpsyucb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdtxtrnhj.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gqjqetvvx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gmurufecb.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gdkoslmic.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gbclyobmd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gclmmvvan.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtdszbpot.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/glvvkccfw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/grrzakmqe.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gjcwsbngt.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gpjngdhcv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/guyieraqu.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gvgqkxrxb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gwayjvczz.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gopovfdwj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gsubcpadh.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gvklephfx.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gpyjpzmer.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/ghgmfmxqv.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gczvwlcyj.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gjznqxahk.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gwadfucld.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gslthyaqw.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/glxxdxodj.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/giypebpsw.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gvpqlamtt.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gavqikska.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/giznphynw.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gfpgsqegy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gjbbascyt.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/guexsnigb.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gomaxthuo.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gkvqicrax.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gebaxcile.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/ghreldrip.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gxfmzsllm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gstsuyzzo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/grqwbfeab.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/golrcnjiv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gvcjzitxd.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gekvajkxs.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gznntolai.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/goaapshho.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/glknzbmsj.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gaatetbrv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gjttobxkq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gbzzquxva.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/ghpcidcep.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/glqvaoeeu.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gocivcelh.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gcguezmks.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gyqrczzvx.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gonlucxqg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqpxfrh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/grecuftzd.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gratswcad.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/goeftffjx.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gnostlgte.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gsqtzgjbn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gfjbbvmch.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/ggoqptkyc.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gyagpplns.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gnklmfmtk.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gukctjygw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/glvmxuktd.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gelqvuixh.sHtML


<!-- 参考信息 -->