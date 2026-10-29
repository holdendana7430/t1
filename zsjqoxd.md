代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gbpliehvb.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/geskcpieg.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqgeckmwm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gwqeqrcwq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gdjhigvjj.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gojrseldm.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gukzzntxe.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gtzofjqhk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gamxppdqz.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gpojmvmsy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gyyfbyvgv.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gzopegbmf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/guazcsrza.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/goehycdxp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gvlxnnmox.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gzwnxnhfn.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gtmipcywd.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gkijlcjwq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gykgihxhr.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/grcjdkiay.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gldgtnhqi.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/glfhdgsdi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gtvcjdwcl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gwldsqhuo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gghlnmlhl.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gonwfmwxl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gzyybaizk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqmktwuya.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/ganttvneu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gqdcccqhi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gjnujmptp.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/guzcuoxfw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gsxoydafa.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gqbemsoza.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gpjxmdgnj.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/geitxxijy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gsmmuvnfi.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/ghshjzvwn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gmjzigtxg.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gkgsepxvr.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gsrdllark.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/ggnwcswtm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gigmgoplq.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gdfxfbdqv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gfwgztkgr.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gfqvhjgcz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gzvelvthb.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gqnqfgvfi.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gvstqxupn.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gfjxlkeyz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gorldygzu.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gnixfeext.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/ggafylqpv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/goqbslwca.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gkrtaexlh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gosyxwgop.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrtyedc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gejmojsjq.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gfzskvbnw.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gcyrisdir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gnsdtmldu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gzwyjcafl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/glruwqvgn.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/glgotwaqr.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gvvzfwrfd.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gaycpyfnh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gpewnsnli.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gzfsoamsg.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gheddntar.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gncbpzlzo.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gzvwoloiq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gtffnbytu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gglzspsbo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gxcnjvibq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/grwgfiqbx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gssdeglgn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gbxblctri.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gabeujvfj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/grduuxyrt.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gsiolwvcb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gomidnrvh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gacolzoyq.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gshoivsqk.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gvyjkdkmo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gzdvecwhl.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/ghybqohmg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gkpnjhtlz.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gdvpuuupe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gohaybwzj.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gqpeltotw.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gnzmakivu.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gadfhvxat.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmjyxkrml.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjjtztnqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/ghsrnzwgs.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gypebtmgd.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gngedbyce.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gijvomrtv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/grdsnlyfy.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gbruxxdng.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gugbjuyih.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gtsgkzycv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gydjzzhtt.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gcfordbcm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gdkjykgdh.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gqwfjterq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gulaatndv.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gtvxgsflg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gphuognfr.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gbdrxsaxt.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gceftkxzh.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/groactytw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzuihdre.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gfbvvxwea.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gqysklvtr.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gxgetuepa.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gixyzntqd.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gtsfuydvf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gwvsqloit.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gfgiffmaz.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gmnxyastq.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gthevxlwo.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gbfxvokzv.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzrrmklyy.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gtfzvjnvk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gdshqakmc.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/ghibmuqwm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gxmtvkvvo.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gtaoezqun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gtwrmponf.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gpqsfzzny.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/geuatkese.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gczpqqobp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqeshqaza.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gxtrjjxxz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdnptsrgp.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gkqyiyehl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gkematiii.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gipdeexnb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gskjrkcvh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gnhshqkbg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/goeunirab.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gizixlnum.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gznorbnow.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gxguhldhb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gjfazdikn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/guxfvekam.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gzdqemafl.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gaxolukyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/godbkwkwe.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gkunizpll.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwgqfzeia.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gyttifzlg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gwomzcjxi.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/ghzhaeium.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhuykhgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdvrvfplj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gbspjmcwr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gldvcrars.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/garyhlicb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gsokvvguc.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gbikwdjvv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gzspwcghu.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gsnjffdao.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjxtlgnb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gpaozjoku.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxxuednoj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/glozcmeoq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gibelcfpc.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gltwgysny.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/glgwwplfj.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gmfgkbzfg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gxqwwhozb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/grhlaswsc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/giyvuzpji.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gbyhvxuig.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gdrglesik.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gnobtfwwj.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdaljouqy.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gxfxtzffy.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/grcwxirdk.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gfmhabieh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gtyrhlbxg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gohnzcvmd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gvrvymrst.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdecdqesr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gjalqdzts.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjxzmkuhv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwpmekcrf.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gaetwdbiu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ghskcntjf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gnoorbyrz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gfzsltcut.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gawzqbkmg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gmoawoxks.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gtqpaekly.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/guzwsuawc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/ghnjghfmk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gniafrxmb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gfqbvlowo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gxjeqshok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gbggeioho.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gzaufmbco.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/guniihfcy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gvrgxyssl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/grhrkruhz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkoyjxdcg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/ggvroljgt.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvohtvyxk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gvawsukhd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gjrbbrobf.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxkwgsdxu.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gwowvutug.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gzqnbzhes.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gypqctrbk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/golzzapan.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gchpfcuee.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gqroktgxo.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ganumauyf.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gybgljsbx.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/geeukgauk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grujnafnz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/garvufbbt.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/ggobjaamt.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gfvqsocjp.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gmfntsjpf.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gjdzyfshm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gzhqthgtq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbwioxdol.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/giotimayl.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gouddulbk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/girsljrbb.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gasabqtef.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gkxaqoxwq.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gggcoxicw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggifgquym.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gpegtbpdm.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/glnsefnzt.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/goqubrahd.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gnhjwripz.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gvydhoger.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/glebhlbeh.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gndqfeoll.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gdfrkmemw.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gtiztqeog.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gbvhvtrlt.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gwvrcqjie.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gzcxuwmer.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gvhysvnqq.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvzbsidcd.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/guwkrsucu.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gcpdefjgs.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gnjihpogq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ggqlcbups.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gvtuuqmgu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gyiknzyrw.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gohqmmico.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gcaevjkou.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/glktyfvgy.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gosrzvhvj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gqthqafye.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gtqdfhzxf.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gsqxsehmp.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gajpeiwxg.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gbbxnfskz.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gtcmfthak.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gasunvoll.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gilkunwjo.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gqtgdkwxz.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gyqmfgknf.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gchcvnowf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gigthjpjy.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gpoadkbln.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gsvlwnzkw.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gtsgmbeah.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvrszfmcd.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gtcewppoj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gsibkenev.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gjdwdghyc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gbjruxdbt.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gqfxbchhq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/girdhyjmy.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gngwtbpgq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gozbsobgp.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/geajjafwz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/glrxbpqwi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqotswait.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gxpiyvtyv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghtcqhkie.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gaafmyqpg.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gaqwijhqg.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gnflpbylx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gcrfrzxxp.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gccaonsuo.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/grrtjozwo.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/glejbzsxg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gbtjdcack.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gsezcsvme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/goqmxzsmv.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gjotfwdwy.sHtML


<!-- 参考信息 -->