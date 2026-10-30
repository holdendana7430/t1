代发 wailian999

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gwniwkdfo.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwswojjcy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwxbumd.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gabnwwmoq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupjqhscq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gktmimjxj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxuijrruj.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxjvlyqxs.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfqdvbbu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjsjxphf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeucxhum.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gdtgrdtpr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gqpddtqet.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/ghgerokzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtbgvpji.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gbsgkdvuz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gnuycphgr.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gafobluri.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gvyoyyvug.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gtrdrkypk.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gfnsnaprl.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjpslegb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrqliwsp.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/ghlstyqnw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocegdxj.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/galpyuijm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/ggzteblzu.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gpooffulp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvttodva.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtoloszc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtftikovt.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpywmxoka.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/glxfdurjd.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbjlqikh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gphqqwqvt.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxwwapfll.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gcvlwxlti.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosroqwrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbjqignq.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gqypnqmrh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrfhidis.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhredemp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdojhhxuu.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gclxqbfmk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqezcdxo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/geujdxijn.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwlzxorj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjnqrvmuy.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gguhihjfm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgevjcwv.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdynwkcmt.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gdpziofzo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gugwudvfv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/guupllpvs.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjlsggbn.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvzntecp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzbjivsp.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/ggffrcxbm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzwxqofj.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpfeioybw.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchpndffi.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/govzzueec.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gwehztybu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grydamlle.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlruykpu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ggyfpnwhn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjhnvvdv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwglspdkj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymycsay.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/goncwkcxp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gspfzhfhu.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmjdetv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gfrysrrxl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgcndnvd.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/glzuqqfvw.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqspwmzfr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagpljsgk.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxgsgzb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjsfhcmm.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaajjbbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkydwsrlm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geobdnbya.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gnfimzdwh.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjrabjd.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gztplddym.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gyaewnivg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmsakfqj.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxlvgpzg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmqvqqwy.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjcvcppz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/guhsbnjdi.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqvpwius.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gucwhytwl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhkqmekm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gtoaumdas.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gblbczlik.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gywufpgkb.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gnaswhukh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/grxunrhzx.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ggshywlim.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfzleim.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/grcsytvjf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyjkdkjg.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwnaztlz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gawaodygu.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpmozhsk.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjdhxrcla.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guftelqoz.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfneiing.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggonyzzkt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gyiowxjij.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdeacton.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/geyvwwdpy.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqbqoxfgv.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpymmkso.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhjzggzu.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/giscxtlcd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmflyjrg.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/giraxpgay.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjatopfr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gossxhcob.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gyloutesy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhwvfbar.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwvloojl.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtknypaxy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxjjwejv.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gggtcikbk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdjukdnjd.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmytugvks.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gmeyzndel.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqodokdfj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gcitgvmlm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmslhmopd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdnclwc.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/giuexukfi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxclabwqi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gceypqfyf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnsmpcmpi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxfodxmh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqvjvgfld.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gitbpcqil.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghywtxasl.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ggspjkppa.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsdmzjtmv.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gxyeenycc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gplboplwy.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyesoctg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gicugzwpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gszcofjah.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfgohqwep.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngzkemaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gqnpgglrq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grgwymvfp.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpuuvxfoi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/giofefoyt.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbylbfobk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkrcvftr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqtukvx.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gvrhepxqj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gtaipfuji.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukffaaol.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/ghyxhzcot.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepbnpvhs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvalkemo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfuqqgou.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/garujawka.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/graucfjdm.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gkuzvmyeq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmjxwdpx.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdfizryh.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlbybdze.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/grgwulgpt.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtbdupkk.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gfubhdooi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddeiyetk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gjwtnwjmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gsswbnpmr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gycxeiiog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrfylyyu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnyenehub.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfwyivsf.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gntfdefkr.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzzhadppi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gkitrjpxn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gywrxjiet.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxxzxxxa.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gmteuwwwm.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gjyychfkb.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoongean.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzijvpjka.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoygosez.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gygzvluek.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gcudvbfkq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwvimbji.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmgnxfad.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gtonvcbhy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcssoxdz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkrxykas.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcuvgvxtj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvelkanny.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/geikiktne.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/ghtmrqfpc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnydxcnx.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvscsiard.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwtjnnnc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gobtbdere.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gjadkzutq.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxespxfc.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqzwjezz.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gmphjbzyj.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcjomnlw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmnhwomq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfilxeiuc.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/grixjodwr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfjcbgvm.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzgjjvuk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ghogdrjze.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwpvlnwg.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkptfjmx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavomishi.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsoaukbt.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqkwaffj.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/grezbeouw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grwfwlhhn.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvsdazyng.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnoymsyk.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gntovbyzc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrmnplbj.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmufdlkvz.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gotsokjgl.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhmoqkv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzejdvke.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gxycmpcza.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtvomaok.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgpzbwjl.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gykzxmvvu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gguytojnc.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsrbrvvd.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgntjimx.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gulegyhen.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gidcihnvi.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gexblcqfm.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gadzrelky.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuqveygi.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljovdhfa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/ggwfgzrjs.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqudahbib.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gszzbwqos.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gfblyaefj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfjwtsdy.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmfwkqey.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gttchcnzr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/grqzkrhiq.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/giyytdods.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grdxakmsm.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/guiissaun.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtnepombq.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gnisdpcdz.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gcgtsvnek.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgaldyy.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzypbixn.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gemxfbxtc.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gluammmjk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gebtgfgnu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgpbqbcq.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggappzbxu.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjycjehaw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmkxfzjv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gurdanibu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbidtgkhr.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gawrxltwa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grglafdwg.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gctuwbfeq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjpaufus.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntfrxkpx.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gzdqithlg.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbfyyrt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkgratue.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvuymhmi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmufyzctb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhqyppkd.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggyvvcxbw.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzayeizzm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiqaijpj.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmgkeknxy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/glsfsaugf.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtllfewa.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/glzrrjfxi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/goejkeerd.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqptlgwxg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqvfwvwe.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gphkoxlzq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdggyimh.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjtwqqwlh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngsknkro.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzeolppx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmzernug.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gweeklpob.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsimjgneg.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gafxiqobt.sHtML


<!-- 参考信息 -->