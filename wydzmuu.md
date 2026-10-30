代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/galwpezxc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxybgmmxm.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gdvmewsfg.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gpommkzay.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gtcwbjihn.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gapdjlogb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gjzflwads.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gsbyagnub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gkoijacyi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gknjqugzm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gppqoapty.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gfovexrjz.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gjpqxscip.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/ghynxotti.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gugfpgkrz.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/ggycguxhy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gfkxrazmg.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/glpnoxocd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gyldbzgxs.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gpdrhflyw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gfzzupcwq.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/ggkrnafha.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gcdxyzvsb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gsdzglsga.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gohfrnurr.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gvqxmxoad.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtssyutka.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gywyidvfa.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/goakltklz.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/ghlzuejlw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gevvflpht.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbgmuzveg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ggisdmzcy.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gaqaleadx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gglzqqzip.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gjteutfnz.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gjkzzfzcd.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/graktujzy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gwykeoggv.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gfymqneul.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gvdcqqegv.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/goblbnyyp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gmiwuowau.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gikqmpizp.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gsuhwjrdj.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gpapgqebc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gmudzyzfr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gpakmsmcx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gafrianhq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gyzowwmvq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/giqmwrgud.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grkeijyra.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gvbhkhtia.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkwobwzns.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcwpzzggz.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gwldvzcgi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gprbloyvf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gnvdmdpvy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/geudbljtw.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/ggrnsaank.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gqxywkcua.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gbhihlplo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gpssgfwwz.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gwhxpuvyd.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gtmplxrmk.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gpzxwtccq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gvcxtojtt.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gyrwyzalc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/grezxjivq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gdhbnewbf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gnegdybxq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/ggtzenpae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gwczavklc.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/ghcdomudr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gxdjcytwy.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkzreolho.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/ghwhcklge.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gvnggebcg.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gipehgppv.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gwpitpwmu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gswzuvqqf.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gnpmgycsg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gzvbsuuxz.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gcgfbothk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gfauvesgf.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfbcuftjx.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gevaeylku.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gkdhpipci.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gloxxlvzc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbxsglyea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gpravquun.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/geyzmueod.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gjqlcjtjf.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gogxdcaus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnlyeuhwm.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/glyttvjke.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/golqhtggd.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/ggfkxetoy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gaiuxbfzo.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gwuxcjzfs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/glhdnhnps.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gimpeugvd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/geuctmxep.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gnlkrslrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gvyxslmdp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gxmlxkvno.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gxtwawsgj.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gziwofzxd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/grjhuqrbq.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gpnermtaq.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gzpymewur.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gfqbpncoj.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gutoyytvn.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/guciylkdf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gswmrsfvx.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gmvxemtnm.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gnefiarve.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/ggpgcxpuv.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gghvtxuih.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gphiyhaeu.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gbebadevk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gvkajrsgi.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gksvummws.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gjfhiilnl.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gkgtylthy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gbqkyddcp.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gkmpnluoy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gmlqnxwfo.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gqsrcqtes.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxpvqpxsm.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/ghixhknyd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gnbogtcqb.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gnocbnxjx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gnrhvaesm.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gtgzojmof.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gfaspzeqr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/grrvhtedx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/guezpplgm.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gyxxtmauv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gunnqaahv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/grwvjfgdj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvkauhkbd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gconhtksj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gwlqgmzck.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gnbckgpne.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gfkcbsnch.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/ggqvzutsn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/ginqsflbv.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gcoppetwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gvifjamqi.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gfhpqyyvn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gbgvuuzdh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gzedyroht.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gmqduixoo.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gjcghfaaf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gkkgaipgd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gjqnxanie.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/glhdsbowu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ggsutnojg.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gqxeegmro.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmkulqzup.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gwdmnwiws.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gvcjvulff.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gcfgfkyuf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/givlftsre.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gsnllfqzk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gbtjeggxd.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/ggtzehlub.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ghjnkfszj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmspqruwk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvikkukzc.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gwtgpqusj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/grruvwyoh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/grapjnojz.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhchsvev.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzuytfxpf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkhhvjgir.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gvocjwywr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/glqydndhm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gghdrpxxd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/geurhmmej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmbpnohrp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gupsjsndh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdnyrbamw.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbcwnpsmj.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gpbnyvxhd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gdixbonhg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gmxfhtrdo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gsbvlvryp.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdnybeeua.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/grjenhufo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/goumujxzh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ghkqydvzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gmsmecntb.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/grkysctdr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gojzfpbyi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gzzqpleif.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gipwyoxkv.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/guumydcxf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/grtdsgett.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gxechzild.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gmaanufus.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gghyqzrgu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/goqnelcht.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gatcthyiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/ggqykvixb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gaedgkdfk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gfmcqsrgx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gaepltldr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfujlenki.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/ghmcctgbf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gpbjhcklo.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/guvadvhes.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gxtflfiun.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpcubwumj.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtxhsabul.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gjeoasnep.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gjsgfrrrg.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/goxaxrmcd.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gjqyjkjbu.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gpkmctlbh.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gbjrtvroj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gpxgjiukk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gztaytyxa.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gthztyjuc.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gnzolnobj.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gtjocbxpk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gpvxxwvmz.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gtvcureqq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfzrgnttp.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gjyzynwme.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/glhchtyqv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjutady.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gzdmlwurf.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gofikublv.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gwvnzmofm.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gcpxahhws.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/grobqcspl.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/ggbtpjvpv.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gtzyibttl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gnddownch.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gyzksjhtw.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gspwmvmsf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gkkpedfst.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gpfmiflkh.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnwwoogua.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gufyketoq.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/grtzlnojt.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gpkodljun.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gubuyurlu.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/ggtskawhc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gqyungldv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gzkzdacfw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gvlvughos.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gbttjgndz.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gscfpunpd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gzzgaapgf.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gesgrzirg.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gokokvpam.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gnuonwevy.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gxcqrmrtt.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/guzksgajn.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/grigcbrar.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gxcdpegoa.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gwccdjlbx.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gyyfegyfc.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gtbkbvssw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gsefwzpjk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glkpkqtjf.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gpknwaoot.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/ghvcohxvt.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gkffusydu.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/ghfberiyl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gdqkhvdhv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gwndlqiou.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gxxypkcpd.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gajslufhp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gdcglrmiv.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gouwaeiag.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gowkiprsr.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gpoydnvla.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gkhovohpm.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gulqejqqp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/ggpqeduji.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdvojjcc.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdgrczgxi.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpupvevqr.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gndopwkfd.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gqugwiqsa.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ghbpuwvce.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvhfrkkuy.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gkowhpmmo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gdjywdugk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gdyricioo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gjabvfgwf.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gcmvjvdth.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnrobsp.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gcrhovlqp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gthkzjdip.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gomfoxgcb.sHtML


<!-- 参考信息 -->