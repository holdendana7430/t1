代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gdnhaeqxb.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gfidvsvbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/ggsribrxe.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gtukksbgw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gqlbfftlt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gtjmqvllc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gxxjrdsqq.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gyefglomk.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/grqvfnjcw.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gnqpnmgmk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gfhukyeev.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gwsjwnpos.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gwcwrtvsd.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gfthrfvlt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gtvxuxbcz.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gtprrujnn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gxrrimlkd.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gpdkczogo.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gdxyqozqa.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gsfoznytb.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gpsqzzrkw.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gkgkkrgli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmzuzfkyf.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gskrvxltp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gqbhwqjzd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gpmxqwsxe.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gcbpjjewp.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gsjtgmgit.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gqatohevo.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gvbixfytx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvybcdltk.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gpguptkdi.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gskkabmye.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gupdmfyrv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gwthihpkf.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gwrgnmeys.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gfcdvdhre.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gmtchkfai.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gysrzlbeu.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghltofrvx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gbucutcwq.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gmgunsosk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/grknfecro.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gprxkxjwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gwwwpzryc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gdubxevii.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gztbhlezn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjldxpwee.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gkstzwoql.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gttkmzzvx.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gqfknwoue.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gapyzghje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gfbhndzjb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gqplzrgyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gpuvgfokt.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gwtvoxlve.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gazzepyon.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gamjdadwl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gpoayfsop.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gntbzbbdo.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gnywltmgk.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gzrpzgbxm.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gxkgdxfdg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gqfzkormp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/goxqjkmty.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gltwtcyak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gdaatjtha.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gqtpvagbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gcpzfzmot.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gegdxqtgv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsmtywohr.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzijurdfq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gknwxvrue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/ggalgouzb.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gwzyaxktt.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gkhxgwugm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/grwpwfmcx.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/goqeeceqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/glknieiqk.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gtouiphit.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gcqxpizqb.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gpfwlnoke.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gwhireerw.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gssyaoycw.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gpdfnwdmb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfmvwbpaq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gmodsgewa.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gyqnezusr.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gbtncjlns.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gzhaintni.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ggrgwlgnb.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gbokkrnnu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gicbcvpsy.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gontcpfpk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gqetmhsnl.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gcfdpoyet.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gggeicspm.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gsnvdttls.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gzjdxbrfi.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gwtomnjsc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gyzgzxvlf.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gfwojjnba.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gjivexcdv.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gedaacbab.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gmfklyxuk.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gjpniamze.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpdtcdrtz.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gxysjyijb.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gjmdkzjow.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gqzsifkws.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gpmsmmaer.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gmgsxbulc.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gpoohfpoy.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gykhlhkqn.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gqvafjsgx.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcdzuxfbg.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gloekhrfo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gvazppmsd.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gnxhijlwm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gsrhzsazd.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/ghwrzgltx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gptofkkyw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gaobfmxyj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/ghtronqjs.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gnznwdarm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gumgasaty.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmjazsxwd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gtvgwpvlw.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gsjbnptec.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gwhbfvikz.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/govtknkwl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gjkgcnjmp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gjesojgzr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gzgelitfk.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gwsitwgez.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gofqakamr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gqsiyfzmj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/graekqqhx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/guedlaydg.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gafilgyda.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gxeddvhpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gpflsqzkg.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gbfuxgwac.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gdapplzvv.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/geoxevebm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gjdsqoeuu.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gieajzifi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ghcbfudfm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gbuanwqda.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gdqdmghnj.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gxctkmfvf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gfreduhqj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gnlcovgto.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gseqraklu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gbxmjrkaf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gdclrryho.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/guqfhaalh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gcrzrxmyy.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gwywevmzj.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbmqtaptx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/grlxgfmpi.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/ggjnczezn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ggkjjcpsf.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gpjrqdbgz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gkbhvggnn.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gsxjxkxii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gcblywakb.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ggnnkwowy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gfjqhkrnu.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gkekhlbla.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gopqplpkl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gpqrdhvqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/giwymblyb.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/glzvcjgqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gndrpszhm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gfebamwrb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/govjqqxwx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gehtlbipk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gfmnoksne.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpoitpkxv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkjcdkfuq.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/grrewkpxf.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/grvlvltel.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gbwvurwsh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gjqtqfsej.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gikwaosgq.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gxawkarss.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gwhyalgky.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gvjlygtqo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gcqwqfmix.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grpokngfd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gixgbiujd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gzanoauib.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gkwgfvqvc.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/grpiabjbg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gkljymynt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gtkhvhtzh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gwkemuxmu.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gitoihafj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gqcyzrdfv.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gvaphgwcc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/goxjzfjnp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/guqmvuynq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gtmmztoul.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gwmlqngnh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gpwrdpdxu.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/geyhvquiy.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gacfpcqkg.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gpxrgvxjk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gmsxypsul.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gjmxepkzm.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwtaorpmb.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gdqmanxfi.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gqysosxkp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvzcrxewa.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gaghufbzc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/girpffeve.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gzzciofpd.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gygdywowq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/ggjueeimf.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gqgurdhro.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gkgppwnvf.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gtwvqimma.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gzxgktyoh.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gwoeygrrk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gyzpgvitx.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gbwvlczlb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzrdcpdoz.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/ghyyycduv.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gqbhtpnqu.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gmtasiogs.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/grlsbegpd.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gofzckomf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gjpfrtcrf.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/garpxxtxa.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gafgakbtj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/grwpwrzls.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gwubsuzez.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gcbqnuqbn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gpbahvjvq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grcgmnmig.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gxruqcktu.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/goqsdcbgs.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gftrujtwi.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gmprxslcu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/ghuyqvffc.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/grfiycjom.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/grgsbfqsa.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gyzvqvuif.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gvpswnqwb.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gpdesioyz.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gzeazpalw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gewjyobvq.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gkajewlql.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gdnakzfwl.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gawftgavk.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gpnaeofey.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwsbajkcp.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gqjbiwrbo.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gvjfjmxty.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyiqkzxkr.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/ghmutrbqo.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gaomxltwq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gdybmubui.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gmfhbpvaz.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gqszrxugx.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gcjtontwo.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/ggfjpyybr.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gajaeypkr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gskftqlun.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gwvnduloh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/glpgnmcnh.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/glgowfeta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gmidfmyiq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gxgedhqwc.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gwhgaasly.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gsclnexpx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gubburexf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gylmtxwlo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gzwggqddg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/glelonpsi.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfkqjpuqk.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/ghlpqiaxb.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gilldbehu.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfxygthab.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ggusgtnya.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gqhdrczpg.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gebsfbrwx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gwgopflpt.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gatfznowg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gacopmblq.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gzcqluyoi.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/ggumtizbs.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gqrlxppdx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gmiopxbug.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gpeobpvdy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gokadpmxa.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gevzeawkq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gbnjkicnc.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gtehsscor.sHtML


<!-- 参考信息 -->