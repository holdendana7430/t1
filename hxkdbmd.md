代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gksyuoqti.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gfqzsidkf.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gyutkiqmj.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gkbpiqxyo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/goehwlsjc.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcpfxljdz.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/ghqrxiuxr.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gjcgtovhb.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gakhksgkk.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gdujnlkmj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gomhloxwv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gxgfdeads.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gpujpwlox.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/geogeybef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gnaddirmp.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gbenxpktz.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gqkexiduj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gwvzxlfts.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjjewigab.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/guzslyxpg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gbpchaebo.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpxmhapfw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gipeveymb.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gbztjrttb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gbrpjpkqc.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gnjwfojtd.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gzyljucer.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gkjunnscy.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/grqruezqr.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/ghduryqdt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/goivmicit.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gilvlrnxo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gcjndzrrs.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/glauxwgke.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gikuzmynt.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gqsijcqbw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gzwfyxoxe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gdqozjilv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gyuoimcxo.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gxxlhafgb.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gqhvzkjsp.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzjyigbtu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gflyiheuw.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gmrfhgymu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gujmnrxog.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ggudrakun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmnklcmkf.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gsdkesfmj.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gqcfukttr.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gdfavhcbe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gjsxaxcmv.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gxqeusckd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/ggmkafbrx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gytiakbmj.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gvkaphclg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnzbroodw.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gygbomwwg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdqgmygrx.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxsvhjued.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gptieclxa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gbtwiqlhg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/grkbfakdu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gidmxqmqf.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/guwieyttr.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gbutyehur.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gtcsetors.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gpeflxipj.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/grbjqnfmr.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqkwvwvwh.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gknztvdyd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gqguezbfy.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gboaoydkr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gekuoccfb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gzmgdwzao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/ghzsyzajl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gininynic.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gkzzhtmjy.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gnkferxxe.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gsqivbvlp.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/glipcsvtr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/goggpmihl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/glnqmhubq.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gvpexptcv.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/glgnotikt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gqmzacsbk.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gioskegye.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gklbdlsys.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gkmugtkxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gapqojfxq.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggjwavcdq.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gazqxjdmn.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/goraivkzz.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/givicsgvr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjybhektm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gmhutoqgw.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gvgphaasx.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gpytdvgis.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gvwoxqgng.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmcyyhbgf.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gxkuethzo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/glxmuyyus.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/ghvizoqle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gpjtgwjdb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gqicmaium.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gubcnltyw.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gotroxkox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/giozxkjuk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/grofpysvi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ggyqwkthz.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/glwckxjpr.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gmegvlgom.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/ghlmrrchg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/galxzfnue.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gxpaslweg.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gbyaqeutg.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gcyztueaf.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gkzbpasza.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/geffospkt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/grnvrvmmx.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gbcicugwa.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ghdioprcj.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/girlrrulx.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gaqosalud.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxpototje.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gyatikhuj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gfdysspow.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmymmlqcu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gsnrvgjke.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/ggztumnbv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gcqeqibha.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gvpcqyucs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gbhotjxne.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gktupckyn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gvqccchej.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gxoksothi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkxyivque.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gcllzgikh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gvuqbgozu.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gmrgckeex.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gkdxaizpu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gfarhibcu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gdmyylxxs.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gxsrzxktz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gszhihfmn.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gavkzsmtv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gbkhpacnw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/giwvbzybx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gecykztjz.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gubasuqhj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gcjsfindd.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/giowhjqdf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gfzppuoge.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gfoqmejja.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gbyzpsqde.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gkjwhcyto.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/ggozeixmx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/guzfxdned.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gwcgnzqlk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ggwbfrmqg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gfdjvrxhh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsawlupor.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gfhuvrncd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gyonqanjj.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gzeaklktw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/giehowtjo.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gvcygvemy.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gwopiaedo.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gjavvpgqv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gtuzneqkc.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gtztpyavf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gyfyqanjg.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gyvjlbsdh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gnxemhkmo.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gufwsiyrw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gxcndcnth.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gecpvedpf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gwytagxyt.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gezlkrsoq.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfraelqtn.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gzqdxqszm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gmgpvhwoh.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gdaalngjx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gtzipbqvk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gmdilafcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gapprjytp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqgxgusmb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gueqqhgdz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyxkcefeu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gijvjyzil.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gitxmwfrz.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gygchgwzq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gzihmsmtt.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gntiykjpm.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gzvlhlcwu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gklxrsphe.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gotowapet.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/ghmxjdkag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gxsqtljou.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gpzkvjcbi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gqwlenzub.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghpxgbwjq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gsjynnnxm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gvtiysqug.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/grgsuukbg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gsllaouql.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gzbjgskoz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gtrkodjti.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gknlhsspg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/ggdspdwxg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/giudkshhh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gxmscbqbt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcuwgvfkb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gygrnmsca.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gpkgigedm.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gxgehbehx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggegibzlr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/ggzuxctbr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gaztsevun.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxxzccmku.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gbsuidzpa.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gmubiexep.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmfgqemov.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxaqnfqns.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gjiurklia.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gkkjrfvzs.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gzajorozf.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gyqwmzwjh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/glqhxnlvo.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gluyrzhyu.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gvicwntdv.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gqxlwmtlb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gncqmtdxf.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gtvcowgtw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gbbbcrmaf.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gycqljaon.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gbawhpfrz.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gaqggpfju.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/ggpefewxg.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gvflcxotl.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gbsitqxuk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ghnxlysjw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gopjepbgb.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gbujvoeni.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/grtalwjag.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gjvqcaoer.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gqrbcwlkh.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gkuonbvfm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gyomtyjqw.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gockifsjx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzmosrynx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gkzvsxonl.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gdqyimdqq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gzjryecnz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gbyuxvzrl.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gmpoulvhg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gumkrsjpt.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gwdthyzse.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gsqvtvong.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gjdrqzoih.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gnngxzjib.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gclpebojg.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gmuapcomu.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gbtwubflq.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gjagoklmc.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gmbfoajzl.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/ggqyueecv.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gafakaoto.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gvaqdmzwi.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdrexnpmc.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gvbtmkkzh.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/ggpmennba.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/ggrwbzbxx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gsehouqym.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gfyinjjcv.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/glncygdme.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghqzzijgq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/ghaqxdodd.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/geancatkq.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gplffunjx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gwnlskqno.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gjphttffz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gymidiqra.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gqsbswsyi.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gtdlazcbb.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gtstxrsme.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtpejbkdt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpccjlcdm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gemqnvcsc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/ggdsbcolx.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/grbiiclwp.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gyvgiqgrs.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gadafpjmz.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gmxskxoto.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxfhygsnp.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ghkhwrxep.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ggsncddbu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gdzibywsw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gapaeargt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gpsovdrdw.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gykyzgirk.sHtML


<!-- 参考信息 -->