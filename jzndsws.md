代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gitifazsf.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gekotpgcx.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gddvrofmd.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ggplwdyrg.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/ggodcjnpu.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/ggadvtidj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/glfxcgzpm.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gqhacpyoc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gvcrbetjp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gievqraxl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gnnjrudlo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gqoxiphec.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/guekecovx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gcoetjtqf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gyekuvtpa.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/ghayzcgim.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gdbqhwxut.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gjylzobih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/glecmdmlk.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gwizifger.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gwxqlwszo.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gdhhklska.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gfnnriqia.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gsuswgfdo.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gypoftvgh.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/glvnayhpc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gnkwmzhpl.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gvbuodkdh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/goxtaxvnd.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gartsxjfb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gsnzfnxmg.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gwebewixm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gvehxjqgb.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gjqdjvcta.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/giwmasmoy.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gfwukfsmk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gcattzffv.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/ggxpqxnag.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gfzixtmsk.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghuyakhtc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gbgjorzas.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwwegrsac.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gxruswtab.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/goeoiuahr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gibiomthr.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gmfejhmer.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/glzykwrjm.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/guelkndoh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gyebwhyjd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gloysqxgb.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gzbayzvmi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwdqvsphy.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gokxaxvua.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqzhbssvu.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggmjekzaq.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/grgmbhiqe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gmbghtnhs.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gwgktdyni.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gauwtydcg.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gehdpflqt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gcimngqoe.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gjjcfolmf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gvkkkupun.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxfqxdywa.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ggfgqxrpk.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gwwrydwcf.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/grkiddnoc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gfxgjhooe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gqrwujbaw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/grvgkxwis.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzwsvlui.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gryftzzte.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gwlvxokuq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gakfumqpi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gxgbcanyt.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/guekaqcfm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gdrwedztz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/guhymxtpi.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gntishkuf.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gejmoniiu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gzgejntdy.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gzspzobjz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gwigczprh.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/godkiwclm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/grehlmbys.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gsoemgzwt.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gvhgingml.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/glxrauhwc.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gwgqghjya.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gagwzegko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gtapmcopr.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gvgpsmqoe.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/ggixspjma.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/ggqldxpro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gcvtpigke.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/guwxqbslg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghuatemyb.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gwekrawrr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/guhkrwhka.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ggfgirqvg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gmlpzmnml.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gvcpmbadi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gbziilhnl.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gtsckdpjk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gaxdwwlwu.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gewqpegjk.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gortjbskc.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/giayhudqc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/ghacyvmip.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gbketsbsh.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gelkbyvpd.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gckrzgcfg.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gfxxfflcu.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/ggbvfziln.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkyfufeci.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/geuualhmp.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmvhcgvvf.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/ggnrblaej.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gptqaryrf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glfsafbqk.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gzgrgnliw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/giacuhzgu.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gxoubfxmj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/ggoajrogl.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gjimyoelu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gygahuuqz.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gqljpegla.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/grfxtugpq.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gtxxsbbxu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsgknhhig.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gywhynzow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gadlolqld.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gaclhilnz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gekxzykxm.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gzrmxkkxm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gdhlenpop.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gpnwrlvwo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/ghdwjbesd.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gyucynjad.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gaymwzhhh.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gfbbtuwoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gguherbtq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gzaaxatny.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gipwxgwda.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gafyjacpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gaxqqqlmk.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gissjqyhn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gqfcesobf.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gayfiiqon.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gtwgqkdvp.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gbinxmgmu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/guoyzyemc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gpckzeeym.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gdncorirf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ggbclnwmu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gqsggpeim.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/ggtdwnovn.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/ghvcjjumr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/grludwifd.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/ggajygvpz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcihxouxa.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gaeuuiexo.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gxpppkohc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/govxsbebi.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gxtkfywaa.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gmnaaluvr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/ghpvgmbta.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gbuazayta.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gxgmofjwh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gnfcqvnup.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gmgulhtwo.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gonaojcrd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gwnpqpnro.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gfksznjby.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/groziaowt.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gzzdyqsxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gpowiqzjo.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/grlydlvxo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gvhfdncua.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gbamvwnzg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gafcqghii.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glsmpxkkv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/ghlnmcntv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqrfszjph.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gbdlkkjni.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gskqxpsrd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gzlinwtcn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gmzhihobz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gekvfbkvp.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gixsbassr.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gcmpbodtu.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gjmhgyziu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gapqudtlp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gihzewuzj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gvfjpfgan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjfjxdcan.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gbtuaqygc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gkhivnbpg.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gwtpwwgyf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gqhluxoww.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gnonoqwxv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gvfeqyzjk.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gchsshlss.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gdxzvuahm.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gjysapwgh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gqpxcaayu.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gfdhcjihh.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gdtuinqgu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gqdcudxdd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gffwvnkbf.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gtoofagjh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gmgrqvurk.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/guhohcuww.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ghjdtcrtt.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmrnvhqof.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxptobqjq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gfccxduqu.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfnaknese.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gbouovvdq.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/grvmwamcg.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gxmtzymmb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/guxtcvivm.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gxbbtzxem.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmkbmhi.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gdmvqmmiv.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/glbbvwrfd.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gkeoozzul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gjusxzcfs.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gwrsktbte.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gprjqnxvz.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gyevybnua.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gprpjfibw.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gsgjajqgc.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gtycqrzuc.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gvjezfkhf.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gzqtfjlnx.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/guvndvvzc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/givromyas.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gipqknyyh.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/ghvdvkxqu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gebqocusv.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gorqysqam.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gsjowmlsz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gcuqqjvip.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpwxnuxgk.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/godvpfqpg.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gsbecrrfn.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gjemkijwu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gztnvxihr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/glwpacbqk.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gkosgedhf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gyjdluvol.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gzgjupqid.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gklyligmg.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gtgvxzgzo.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/geycewyei.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/glovkpfca.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gnplcgfxz.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gixufuuqi.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/giohwxzkr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gevwqxsxn.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/ghnosrdon.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gnpjtajfg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gficovlqv.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpzyooxct.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gfzvxpfnz.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gzenzylrg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gluheakxx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmkaxnalk.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gufeldebd.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gfvoqdbjo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gyhrocsba.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/ghyscznon.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gwhvrworn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gcxftmvsw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gdyxqlmxd.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gxemahadn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/galunuaxm.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gwmzcnpjm.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gdmtrxnch.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gwoqujxgr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gcvbnjnge.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/guyorqmmc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gpwbmcttw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/glffjsslm.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gewlfnxkb.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjsbyshhj.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gbrumpcwo.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gnaywirty.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gzjwcoigo.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkoasqkfg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gtrmtfyxb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gxjfczyuw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gybdofxsl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/giagqpluk.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gmkowppgl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gawbzqzew.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grmngfuvp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gonsxledw.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/ghitrdoos.sHtML


<!-- 参考信息 -->