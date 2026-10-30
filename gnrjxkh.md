代发 wailian999

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gfpwfsevw.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtpvxsvsh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gzyaddqrb.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gtytmxfcz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gcnwxjoec.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxagxxdk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyrfpiqv.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gawjbomgo.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/goknqojwi.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwarpydpg.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gtmzklkpr.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdtcybfjx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycgzqrat.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gawhzxspk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtahpaiv.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/guoxwraly.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchqkpgwz.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbrbobpr.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmfbmotyf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwszhsvju.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/genbasyge.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghhfgojjm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqfeideuf.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfredfxpe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/girgacohk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrjgzgjw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/grcuzyhkg.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcbniee.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjusbfy.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmlxocs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grltlyrld.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gscqjgdgq.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/grkewywzw.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbscrjqjn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfnryswt.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/grmkxgoxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkztwhutb.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glvymzdlu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhdvypwt.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gzxxcjhsz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gileiyjbj.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gzqosvebb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfplepuny.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gcmhbnlrv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbehevaz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gavjvlqjk.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugzulozn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glovlnnhd.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvjzgbe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gimhuuksh.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyovjeclh.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gnjyyomcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkgtqssuc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvnwkdws.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gmparufki.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gxaotgiaf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazdqfsxe.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruhkhglo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gttctvswz.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfiigxgd.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfpuzbwf.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmygqyhgl.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwxhyrgcs.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghhempgrq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gjulxbdlj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gahbjaxyg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghetwzmnh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gwohyfetr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhsbygsy.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gbskyudjq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdqejnndg.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwoocgdh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/ghdodumal.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufyijxd.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gckhfhsvh.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvjsfqh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtrezzigj.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlhxqjb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqqtccti.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/grcczcfjb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gaciarzyr.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggxznvtzn.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlitnyt.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gfgcgpsac.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghszozieq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwxojhemu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvauaalkn.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcnsbnuux.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxmgdcpqa.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glvreqphm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzpcpbqb.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gvmdnxmxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbazvvyu.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxxxupuk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvtyyexl.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmdrrcyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/golnkbkbr.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxitnkpgr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbuyoezx.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gqhsoufdn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgxxgrce.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/giqflnhtc.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gsrlcuehg.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmjvwatn.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gnkeuhsdd.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gcxzkcxql.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqhhqejr.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeyuviqu.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gagiphlpy.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghasmaiet.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcinsaqxg.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyvkvrzk.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpxwwnfw.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/giceiuidh.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gdiffzmqe.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzstjpqc.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gygtcnywf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcgkbxmyy.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/geprhrnbi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gokyhgwfl.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gesokivfh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gszrdaevh.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gvndunnsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxcknyqj.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/glwngjtbk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkuxebuyq.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gftcfqscs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeniclgy.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ggslrcmhk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gkhghbavy.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggfblhktb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gpajlotjg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbfjqupkg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgmvcrrw.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwcxeddu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsejgnji.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/grdrcuuwo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjlqrfwp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdaarjqbq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gflepgaql.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbsjwpes.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gssjbgsxp.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ghmqtavzn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrfjilvw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/godsqvwso.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtkluxali.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/guhszuxmy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gterdrusa.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gktcjmgoo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixjlbdel.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/greluyofi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohvroms.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gcqguwwie.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gujaywfzy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gncvofccc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmgoqrvp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmfttntc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbhynclc.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gecdqaceq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmorzka.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggmkyvpqj.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfiyyzk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnruqtsea.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjxiqxer.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghmcptvhs.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gihumekpo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbpzyawem.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gfehrcauc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/grnwqgqdq.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gflakcbzt.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlfysuqa.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gymriphjg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjzlwjxb.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gixepwutw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gzhcwcrom.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/giulketat.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gzusasoqs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrudvlfz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvocdmo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxfqptbnd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqvahdom.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gpvppyzzl.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofwhsek.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxxxlcqt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gvaquujae.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gyrorcvpu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqavjdlvu.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/grlmjculv.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtkkxtuj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapgrsgbt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdkqzxip.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gesmshzpi.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gxadrrchx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjtlnrgq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpfiqcoz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/geoxcfgok.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gynsyvtru.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdstnzbbe.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyrgrsfr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtldixeng.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuzsvayi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/ganpisqar.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlgiqnfu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfgcohxy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gpcsmnmky.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gsvuleddi.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gcqujbtgf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyrocypd.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmojjufs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gromfbwbw.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdlgwebcf.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcwrkvft.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjzloaml.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gakpkguee.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gszvgfcnq.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/glrjbcfdc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmvjvtih.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaklnwoc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjtjhspb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnqbjmrp.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtozfwmh.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/grgnrrcfg.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gfspjtyoq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtflmubkk.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmoewmjt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gasngakjk.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gqedlymbj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorrvycwh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/glimkcive.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfskffyq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuodvahx.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gmnuqylbd.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeivhgmc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytjnndcy.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqibpghs.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdijdruu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlnnwutp.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezwjigde.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gcngorpvt.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gagjnvozf.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxerfvshn.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoacfhgq.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvetjvtwy.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbsygvwm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuaxmdfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/grfnhrjmn.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqqnnch.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gnqyufzxu.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gywijvebw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzgbegho.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbenwjcqi.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gziqtuiuz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfrxcwev.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gbrhgvhbp.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnydzffa.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpojpvjlh.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/girnuthmk.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjfbhbl.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gverqtzsn.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkoubzhc.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glffkujhf.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gfjlxszld.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gvmuklgnh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/glhqcrohr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqvchlaf.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpokfuvjk.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbtlcgwdo.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeqqoant.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/greareooa.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsklolijb.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzmgibgbg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyngawswj.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gkwbkekfw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkxkuwezw.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkqgsalvq.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/ginepsgzu.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpacqifa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzerwktxn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhmpyno.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrvamjhq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuthejfd.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaqopihvw.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggggvcrxy.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrnrkclb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsdehztl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqejfpgu.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gvjftohou.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmwcjpxz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnfmbtyw.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gcduotiqj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnutehts.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gcvpgmeyp.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzygsdle.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpdosefa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtdhcoce.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/giiaurhjj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gsewnakzm.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/guggcxjxf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvboozqb.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gfygfpxnp.sHtML


<!-- 参考信息 -->