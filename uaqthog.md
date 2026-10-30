代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gjxeicygv.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gwhzmqgqx.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxbmxgitm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gbxzfeben.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gvarvicxs.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/grczymorj.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/goehcxcmv.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gzvcdjlqy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gnjtnmwiy.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gxglmgnco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/giqgsixau.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/grcivdyte.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/geyyplcya.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gmjtiufhx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/goxgqedhh.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gfesdfjht.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/glsasjuvc.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gjcsghzhp.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/ghfyiwhns.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gaoxzqjgh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gfdzjcewp.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gegfdosqa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/grkhuauvr.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gnlfpyicd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/ghzzpmica.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gxbnyqugh.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gxhomivfa.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gnplcyfas.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/ghtpeeusb.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gahoryjwn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gxhojysyi.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gdebxgwkg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/ggeazzzgb.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gleriweef.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/grtumilot.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbzvppvwe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gjmgabiaz.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/glpzmduaa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/glklwqcdt.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gttyzfqsr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/goubhuulr.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gjtedvnmh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gdjsleoat.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gnbdvapst.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gmuotepgp.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gyuucoark.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ggusbclob.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gxjpuixmy.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gmgihdzlc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/glxetdwut.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gmwyjkbbw.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gcjzrceqi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/ghoggwdhg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gfiufdmrs.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gozfvdjrv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpmsivceg.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gizdqvyio.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwmvzuwlv.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gviyuhzhl.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gszwqumag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/glavzowmo.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gdonfxnty.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gagtitewi.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gtfsnwyfa.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gbtuxlhhu.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gtzudlzwn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gdgxujcon.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gbgupplpx.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/glcnufobu.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gaqebwsks.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gpvyyonyd.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gfboatmvl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gbjsvsyzc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/goemulxwt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gfkdsrtqy.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gqhgmtgpa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/glfjxcaix.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gvhryjixj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gzipmibfk.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfnazpvey.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gnavmthlq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gecrcsvzc.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/guzytorgc.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gjrbbkjdp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gucosfmhq.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gqkchassb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gcxaopsoo.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqhdgbnzn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gowpkiclf.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gyopeurcp.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ghevzgmrq.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gotwbxiie.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gkvxjcbbx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gddpfzhgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gqfrjxrvh.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnrghagla.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/goonuupmf.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gjnmotyps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/ggmdvwznv.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/ghjosmwop.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gaizaqodf.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gdldyicbr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gegdtuflo.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gltrjvoyq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gneacjneu.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gqilfwtsj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gwtmetwlt.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gznnegfnc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gomshfvme.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gjesxxexu.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gyljzrxah.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gyeuzdgzx.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gijvdkbrq.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gvqtpjaso.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbsdxlzfq.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gxviedcbv.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/grzpkxfgy.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gvkubxorp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gegubwnpv.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gtlpfklxp.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gikexemsz.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gpvpluxwn.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gxzjvedrl.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdwdasonp.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/giryykxer.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gvyzgbzdm.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggpdizygn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gwgrwuauk.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gejzirswj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gmfmlsdfw.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gmezsuoxy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gvgfjfdgj.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/giuhgmzub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gulzwjktw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gbrasfbky.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gobipyyww.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gjmpxypxi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/glocezbfv.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gozazkupk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/giktgcpsg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/geeuunehp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gsczeygmq.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gbuwuaniq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gnuznswxi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gpqqysfas.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/guuzlkvhz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gmlinhrzp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gpbcxydif.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gblntoyak.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/ghwizjwwq.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gtvelaudl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gggoajzcg.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/glqasefva.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gdjcpwenc.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gqxeytkbw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gsgprcpzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/ghsxsawik.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gucxakoyr.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzqwidpjc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/glhddmycn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gedmnaiaw.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gqbxuxoxy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gjwfzjgtr.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gkweonbqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjzjhumqc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gbdolgxvs.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gutygslyo.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/grfqpveuq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxbunzm.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gwrbytxik.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gnfgtnfud.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/grhiozqzt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gagrqnrqo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/ghpemoxkg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/grzxpycdk.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gxtscvffj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/ghgogfgqp.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gxiqlbfhl.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/govtgiqtd.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/ghkeszhwc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gujnvyuch.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gkdgcipsq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gwcwyeunj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gwjzvafoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gcbktgvvb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfhlsqjxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gacwlnztp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gckslkemt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guiohrfiw.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gzhlmpxio.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gljwdfhdf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gcwgussgj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/ggvtsqinv.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/glvlpgvtn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gclawmakx.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/ggtxtrzab.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/ggllieeqh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gqpioqxjf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gdmrbgicu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/glhkoitui.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/getlbjmjj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/ggtekisyh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gijtkflpj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gxayvsbka.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gskwpysjs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gftcoebfh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gpkcgpiad.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gogojqdkd.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/glvyyqjrq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gpodwvefw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gemfoccmf.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gzkqrirly.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gkrdofrbz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gvxiiauli.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gtehjxeij.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gcjwhwewa.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gblmvnmmz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gokqbktfx.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyirkxfvn.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gthfnxssq.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gvtqbywgc.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxgpmcpmp.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpahcrvze.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/grdlbqfes.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gzkgwmpbm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghujvgbwh.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/getkfiaug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/guxcqspne.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gbvpiuhxa.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gjftovmld.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gwkuyuitt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/grjdnnmmh.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/grledxwmy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gsuefspvr.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gzugmlspm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnniaixvp.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gzgoeubof.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gqircpefo.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gfxjbmxaw.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/glnwgcjza.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gsosviykx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/ginlknntb.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gwmimcysc.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gddxnbehx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gbeaoxdep.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gvdhabbez.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gchilpqug.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/givmpgsve.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcufelasc.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gkisjjkuo.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gmkgxunkr.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/glididxqu.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/govptzuhl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gnlhwwekk.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gkeonaqbd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/ggacqrktc.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gfpaipifv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/grxxeduph.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/guywtfhxr.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gayqacfpt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gmmrjfuge.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/ghuhqkdqg.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gkndywdfc.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gmhchjxhl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqegmbwhr.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gtyegzobs.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/goobtfvdq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gvcgebaqh.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gxlkfxzjm.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/ghnrvvtxb.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gwqmhmafd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/guwlupakh.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmapuvbue.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gvbfelldr.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdggtqlme.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghrvfyoma.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gbeffxwlw.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gwidnsbla.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gyvvkfslj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gkrsibtbd.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gdapcolgp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gnuuvsjpr.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gelhntoaa.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqirguvm.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gymoobvim.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/glvxxvntt.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdyvbvfgy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/glsuzhvnj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/geqapogcv.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/grkkqsrds.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/givwiuyjo.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/glirrrkkq.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/grvyddtlc.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdxqrmhhp.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/grsfejyfk.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gfuxdelzv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/guebvxiwm.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gzbasndsh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gxjvtsfxg.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gglcwohjt.sHtML


<!-- 参考信息 -->