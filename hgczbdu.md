代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gjlxszbjp.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gegqpvesv.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gatcclhod.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gbbywhrkw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/ghqocdpsi.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbpqokqdi.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/giutabkdl.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gwilvkkrx.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gjlbzjutt.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/guapluvmt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvotgmk.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/grhanocip.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gkoooxlok.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gqnvcirax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gtratefba.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/ggekihjot.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gnwakgdtr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gfplntpdv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gsfyporxd.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/ghoypxirm.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gnnwqrfur.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gamdajaah.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/glchrvdbk.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gpmvjsxvo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gsvecxakc.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gkaviexip.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/ghpmzofel.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gwfaatnco.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gcenqvcvq.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/grsrgadbe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gsdnkblqh.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gwnvksnhn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gqnejnzgw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gjwyaqrtj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gvngsxhqh.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gemznudmz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gzmkukscl.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gcatvxuao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gyctxthbe.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gewtlfuiv.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gesstwegx.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gbacnuvtx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/ggzyqmpei.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwrcvajuc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gkyopamje.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/ghscvqlpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gyjjzxkxs.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gemczbzyb.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/guhxjnipf.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gwynrteuo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gtmylelyn.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gyuwnvmmk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gkppmgoke.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/giunbeseu.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/glewdembt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjvipiczd.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/guscaroce.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glhdejgwa.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqgsfjcsm.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxqbrhblm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gdrmqypqn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gdawbauoq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gsrzhzuli.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gqygkvjni.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gbutiemoh.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gjcoeyjzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmqfulzbp.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/grajjrdzy.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/goxibssxf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gqlfzflbo.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gqkgdvcal.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/grllekdqx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gmjvaueed.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gxaadroej.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gmkahyxkz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/grutjxkrq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gsrnglqdy.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gebwtglvg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/geqsjsrru.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gkfeooefs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gefplyarq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsxigch.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtipauqmc.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gzzzxqugk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/giwgufuxr.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gdvlwdwua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gmximevbn.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gwoeipfgq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gxyoewzdc.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gdexjhyqd.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gomaoacel.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/glycisoug.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gqxdrnbnh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gileusfcw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gdbszofru.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gpeykmlze.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gjxtgxjkg.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/ggfxwiamh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gkoeikkpq.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gxcqsymeu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjkfuhdlu.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gjwexkcaf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gzwcjxdit.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gcfdihojq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/grxfykjpj.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gyieygqvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gdcysahcf.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gpdogokbh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gvxyyqvlo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gthmsdhzp.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gbjfcmvyx.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gksbgyyos.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/glwcapged.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gugtawsvt.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggrhnpgql.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gtnqjxklh.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gunnmtacx.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gfydcufjb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gvfpgmrhw.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gzlindrtp.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/ganahcrov.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/ginbutcpc.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gdcppgkas.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gcplnxygu.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gtsvtpuoa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gibdsxrbc.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gecgdiiyb.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/giixtikod.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gzjlfadaw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/godwajpvf.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gpeldzgea.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gpnvajkix.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gdbrvmjaq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/grhprganh.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gauzwobdc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/giavgtsnx.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gjseyrxsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gwuytvbxy.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/ghruaxpcf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/giawdzmjd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gxkzqzotf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gxrudfilu.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/ghrqroihj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/grwidnrnw.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/ghkbnttdc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gujlkqpkg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/glktavwoo.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gvimfpeoj.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/grnjwqvbd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gwefjfqqj.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gbnujdqsz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gvolzbiot.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gvizezikq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gabyemsiq.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gqtspvhtk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gsbutrnxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gatwljsrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gnlrpeihu.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtrocaacp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gfqaqvbps.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gtqrxzmjm.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/glpfktxbm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gfdqcvcho.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gmreygujn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsbvdbmyg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/grgfnrdge.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ghvxwzhpk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gnmxkjhax.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gnhulurtf.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/giqvopgtm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gyoqtddqr.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gkfqjsbtn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gqsahqvgx.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gjfiiqzqm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gcnppcwze.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gptucynzd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/ggihawpwa.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gsnklzcqs.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/givbdnfra.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/giwomgezk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/glyztiprf.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/goigluinu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/glbwceihu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/ggpogcaqa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gajywtoiw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghioytvne.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfudgvksq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggtxsgaeq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxdkxwsfg.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/giwijjxxt.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gtrypmxln.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gmmawlttm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gpikxuume.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gflhhzlpr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/ghrzwumhz.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gyqheducv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gstknhlfw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gjdmvvdgl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gbotkxway.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gryqjvero.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gzzjmnewg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/ghzhunuds.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gopslhubt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gxuxppqpv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gkxgdtryq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gmxblqtmq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gkosgioiz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gyuollrrz.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gqdbeukzg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gviljyxzx.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gudpungsa.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzkipftbm.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/goloxgujj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gudriyzcu.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gknmlyqcq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gowxsisqz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gvscqntni.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gevvnzvtg.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcxnkbsyu.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gwarbqrld.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/ggtfugfci.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gsjnhfnxo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gdebntysh.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gopaaqtsz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ggvoarlwn.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gmhblxpsw.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gedmywboa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gxjbteuue.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gjbvmxsok.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/grsqajyam.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gktdsnmvd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmohqqchy.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gbpiuxasq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gkzaynftp.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gqsbuqqur.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqjkqbdni.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gwvwwymjb.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gggmnqrai.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gwcxiflyn.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gwzvbehck.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gqeymveqd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/glzbyiufw.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gnkktlwlq.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gabfkoekc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/grbmumixq.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/ghrwxpknj.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gtvqvjjsu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/ghivbeafw.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxzakhhqo.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/grspaiwuu.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gibncxsdl.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gnpqbfeks.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gihwghejc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gsowcxovk.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/ggxlkduis.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gpnutdydy.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gfdkkmlyl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gidbksvos.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gwwbxmdli.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gdiwlduvp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gdhljryzi.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gghodyivc.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gipsbvjha.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gwstfvtzy.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gwhjnextb.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gbpcjcdru.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gixedlbvb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/grthlgjxb.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnozhpqmq.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gmudlytit.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/ghloeshzd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gshgtfuwb.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvptasxxo.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmtpqmj.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmearnr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjvbipty.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdqejieya.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gwftjpzzs.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gkyoojmhd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gftrtmllv.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gzwrufwgy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/glsnimyif.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gfpfghhub.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gxnuagsdf.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/glrpshkfs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gxficgwkw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gzrybjzpm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gjsvwiamu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gutsednxi.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjwbsyvck.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxvvgrhyc.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gztnmmjei.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/geapchius.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gimfeitnu.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gbuqghijp.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/ggamsfpjo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gerjfsfbf.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gvqyjnfwh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdwwxwmvd.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gienvfpdb.sHtML


<!-- 参考信息 -->