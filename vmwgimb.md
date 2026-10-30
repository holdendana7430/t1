代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gakpnzwdl.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gkzqxgqbk.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcqndindu.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gswgilgsd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gctjsjxwn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/grwdgzmfw.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gaqmvnzoh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/glmyorfby.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gfxeuwulx.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gnzpuhmre.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gsvpcbzil.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gtbgxvbbz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gvegajjjv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gtzxfoamr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gqizpyqgy.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gvgdssnxy.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gylkngvut.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gxxzefkya.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gzlyadmtl.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gkryfdcsj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gxhckxuad.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gdxvyafis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gmuzbvluj.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gsosgaxhw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gkdkupqtb.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gmmwfybqb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbcwhzktu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gcoyfyiig.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gnhzdblna.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gxmwimvew.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gxiklforn.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gmlywsohm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/ggqkcokjj.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gezejwlyk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gkpttvdxp.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gnaxvnhsi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gxjvqyypy.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gmsqonaxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/guwaajyxa.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gwsaornfg.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gjbheymen.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/grjxlfwti.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gluswjoxt.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ghenzxprs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gzkphhemv.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gbusaxdla.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gfjekhvbd.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gqqbkadzx.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/grawfxrrq.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/ghyohomos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gxmxpmslo.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gemsavuto.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gxgyfneys.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gfjcdccut.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gjhwbxpra.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdbrrrevm.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gwtdbjbft.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gciclldar.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqqcyfkpd.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gdrafhhno.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gpidzxlbb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gsgymmatz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gxbpvgrls.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gymbkexlj.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gysvkapxd.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gmefauveq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gdtxestzn.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/ggjvrwsvv.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gsseuldfq.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gyymjebgh.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gbfndodxb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gipfbrwbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/goeifnkej.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gcldwabrf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gdimhfomd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gxybnjnxn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/geecpnscp.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gzaklycgf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gdanoimfx.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmginzqzr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gtcreeznu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gbpmlkymu.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/ggrgafndc.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gzdudyneq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gojtgqhep.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gvonejbpj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gmiqdpbhr.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gpkrbqkxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gestcjytz.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gojjtrucr.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gjffnjoke.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gzofhywaj.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gutmysshv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ggiubverl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gfjvadlch.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gspsidjyo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gvvtnmhet.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gtlbsckdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gzjjegepn.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gobsvlctw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/grftfjdgg.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gyyhgnxiy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gxinszadq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gkmibvito.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gfuteeuxj.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gnboxohsu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gqadkprjo.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gugwmxjch.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gaxhctawn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gqpdgekfa.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gotcfgwwl.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/guhtzntlc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gpzhelclt.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gybpdhuqr.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfgwrglfb.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gsywiyaxk.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gxriquxxh.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/grpblqgoc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gvmhllytk.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gwrdxnbap.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/geqmahmue.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/grlomqsje.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gywgaejqt.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/grpdworpq.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gorjewrbh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/giyelndbm.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggvqljcce.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gcjwnahcb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gyelnnxrg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gbwuvswyv.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gbmbkvdtm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gqohavavh.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/grqhgsolm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtztjqndq.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/genpigszk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvvwwsavt.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gttxougan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/giednotkd.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gwtsdhuln.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gnhlsedqo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/givfyjvjq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gpednpwwv.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gcxmskrfo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gwzjuydjj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gmxytauik.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/grnnmtmuy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gxdywlycb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gkrbkbezz.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/grzmkcgkr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gebmasuxf.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gmsoipurb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/grdrnduab.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/goqgxaabw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gyzefdgeo.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/grynntxup.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glidoddoz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/glrnwfgaf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gctydcrtj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gghhxgtxr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gujlxawib.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gjixxqaqd.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gkeztzvih.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gbuispzwm.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbedzvaby.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvkugxs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/grzerwere.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/grxawcxlp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gtfzsbsdj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gpomffkuf.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gpziiglpp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gdmsgyhfr.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gncfewszn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxsgbdhy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gukzrlgme.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gwjvtgfgb.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gaslkfslu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gfgmufeln.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gaulvhqez.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gefsspigc.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/grxppuzdo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gkqbcqyzo.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gmcqbyrev.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gzjuaffkg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gogpfkulb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gfphelusw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnqziqtyg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gaszyanod.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghyuajczu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyxdfyikm.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gggnmnspj.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gsudrvkqz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gbrgjlcue.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/glvskllsi.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gjtqcrpht.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gwdyyjmmn.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gemncprsa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gzoapbwrx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gsiomsdfm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gnhdiayag.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gdgbamehe.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/goonlqnbo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gktekrkqa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gxzazvrxy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gvlalfnic.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmxumzaua.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gbwaxixis.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gjgxzkhit.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gzwsvbdlu.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gpuaalhvl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gzudvjead.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gkqvcqwbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/geqwkrotn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gsrazsaci.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gjpjstjcx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjgrnglsf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/guzftmelf.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/giscvsatm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gfxggzdbs.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gimunztpu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gaknrqsjp.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gvvdivyqd.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/ggcwwajni.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxhjqxnep.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/ghujjkqww.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gmnbnokyx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gxpvrixtv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gvqtrufvc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gqyzaxrmq.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gjmaxithn.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/giawgwodt.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/grteohowe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gugobqhei.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/guoytufjk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gjaannknu.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gtgjqtlll.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbuvtdhhv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gjwhadaly.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gpwvlyuqj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gjyrwxqxk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/glebffege.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gfgjzvlyw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gdrmtjkhq.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gwihljrvu.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gszwvtazo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/goraejezj.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/ghfarhwsx.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gfxuwqhgt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/ghfvnmxek.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gichcubgr.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/glnjbaafb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gezkxucww.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gaoripprz.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gfxaxqdai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gmetwadny.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gexabfowb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gtqsxjvxg.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gtoyyoyuc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/golhpfnke.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvgmxdrez.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gecydwgin.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gszvflval.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gixqmpkfn.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/glmoumvkw.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/guoyzvlto.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gawnktfbs.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gotjnocim.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/guxjtcflk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ghbwepydc.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gizqpgolw.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gutztqmhb.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gfcbjcbcy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gccfvlewg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghfrgvfpe.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gmnvbfagv.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/ganwubqao.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gbpkyvpbe.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gwmfgfmvu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/ghbsgvnob.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gwfmzjwht.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gfvcykghx.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gmysbszph.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukaunekb.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gpbwtzngg.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/geeotryai.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gttpzmtad.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwvgpongv.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gccawsfnv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gbtxkhzfa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gkhzceuyz.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjxgbugxg.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glqiqvubb.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gdgfjccyd.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gngrgkwvz.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/ghdbuilse.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gazivegmq.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gbovyjqsn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/ghxhfdmgc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggtsqjpwm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/ggsllfakp.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gqnjcwjio.sHtML


<!-- 参考信息 -->