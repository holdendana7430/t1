代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gtgqpeiqu.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/ghmpelwfg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfqxazvlb.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gicrzwxcy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/guxoxlpmq.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gnpelydlu.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwtlnslqa.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gnkgxnzcb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gotzqqoml.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/guizuxqia.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gxgxdueju.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gbtrjdtxj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gbxlmeibj.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gaxakzuio.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gylsbmltt.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gvuvqumcm.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gtiphsfdy.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gcymvioah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gjrcidjlc.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gnrlrztwl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gcudzpzkf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gxlzepftw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gcumaazso.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gadtdphbn.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grkgxrwmj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/ghqeuhxim.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/ganmzuwoo.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzquspkia.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gecuaiybr.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/grbppqaqj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gxzjqeazx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gtyphrnhc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gveusqfuc.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gmktwsssp.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gifcgajdf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gkybygnfh.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gakcurasj.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gelhviqes.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gwqmluqms.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gozfzlpbh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/glrprywbx.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gcivnjvhb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gkwzhzgoo.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/grsuvigyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/guoruejsu.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/glxyyntcz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gfdmlvouv.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/grttbumdk.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ggaxwprzb.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gcbaysncd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/goshxipxx.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/guczrhlkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gmgzfixhz.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gjxgfikgk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gswmqoymd.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gpwroseet.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gitjldmpr.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gkfneztko.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gsnhsulnc.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/grqqzhtzg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gxlxtolvy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gvlpeijxv.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gnpnnsfas.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtkraqfke.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gawzvarbm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwneuybof.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqjsqqtap.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gixqfiyng.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gkrckopki.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gnznyiwta.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gwnihapio.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gampyuwrg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gkcjeomcl.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gzxiyifyp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gaowzjjhe.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gofvefhxr.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gjojdynxu.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gctxurfxr.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gwgnkfopu.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gntvedpmj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gxcozhwor.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gvrpkuhue.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/guezhqtxk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gytzaduxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gasszqwbo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gnhynmrmn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/ghlfutpal.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gifplxrih.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gvnotutff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gvwshojjf.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/giogjkifs.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gaeogyvlc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gybqqsbdq.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/ggcxxmjjb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gxbjaziui.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gqccfuczl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/grxdfonhs.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gyvstuqde.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gbpshxctd.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gmoujpeyh.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gksnxyiww.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/glhyqhzth.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gnxhcgsxe.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gwvchidvt.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gjcwlkzhp.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gatxagutg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/giimchfht.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gtakocyyu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gygwateme.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gxqqhnbhc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gxhmxkpfe.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmqxwztuh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/grdgcgxpu.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/germiyduw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/glpjijnnk.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gbwpnkklx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gzncknsoc.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ggrgnsehi.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gmwfvbqpu.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/grqwczovn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gjleqdbhj.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gqnlxhsus.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gagdpbokv.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gwdqpbuyi.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gfqhthzez.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gyancbfek.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gmctoydny.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gyihpetbb.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gkycuvosd.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gzljzbdsp.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gfrltjznh.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gldkmfges.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gpjbkoscg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gusxshdbo.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gmajzzuuk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/giasmjtvv.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/glykowkzh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gagdqqder.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gqvhsahtv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmiihviey.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gtjwwunvd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gutxhcfnc.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gbafxkoug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gulplptxk.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gvxsafjje.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gsxldzopj.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gyizidtvy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gpdtqvmjh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/ghplgpzvv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gmpjlryxo.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/ggvdvpkhw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gringobzz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcoqjywyo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gerqbsakk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gkunqmldi.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gxkrardgr.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gggjkxtrw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gwuycxynt.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gvculhhgf.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/ggvwfmaur.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gmltqyncs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gtdudnmxl.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gxbwugyfn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gbiidtijo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gjszbxyhc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gkbfmtgwx.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/getwozswu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gwupdscxb.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gtnhkelna.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/glqdgtdyl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ggsyejilc.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gpouvvzut.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gjbztyluf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gqagtbzee.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gtgfnkagf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gpncpvent.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gqmywqtdi.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gogedkkjv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gzbvvpxgj.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/giyuofnxe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gvdfgxwis.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gpcaakakg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gcnbervmq.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpwmsqkgt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/glpqsxhcr.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gefyjtgtm.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/ggbnbzrvu.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gwrpcgpmr.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/glfqygsyr.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gzokhiuix.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gipobkswh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gfyoosmjq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gsshjunkc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbothdnzg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gxnupsqsb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqjwrkwbp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtkhxdw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghccwyvkw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/ghmdatutc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gvekwigof.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/ghmhatval.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gjphecszi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gppygwegf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gabsgommo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/guswaonbj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gjopdozas.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/goekppfvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkvxgffbk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/glejsbakp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/glqgwlwhf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gbnspwcgr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gxaejfvuy.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gbqzkebje.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/grgwwgyfs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gksiemfms.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gtekdcvva.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gnzozclbr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gzysrspty.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/ggatmiddr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdoixzh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gxdmlvqzu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbewzdapq.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/geqrrhegb.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gpojxxebp.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gqzoencce.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/glggrkfaj.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/goriiyhve.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gtbgytzpp.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gelymufaq.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gqtgiwgij.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmziwwo.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gotncffov.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gdrvibzgg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzorxrrnd.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gbnvnnbuk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/giavqnscb.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gvnmwshux.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gkxvbbmap.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gugwxejls.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gfyfwipty.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxxcpqjru.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gnckcgrfk.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/ggtghozpi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gcvjihrct.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gptoevblo.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gfrsaglgj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/geaekuymq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/giwrixhpf.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/ghjqbceqy.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gxwfttflk.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gvhgnmskr.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/ghkxvcqsl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gjzldreoo.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gnvyilasg.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gibrblbnx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/grgkmncqp.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/griumsoqi.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gjqtlgvpy.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gnxvbxhwd.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gflavnljp.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gzspcmkux.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gwktocvcr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/goovzyexn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfbxuhwfs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzkjybu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/goojtdnqc.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gstzsjhbi.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gztobahnz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/goghyhdra.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gdqassjhh.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gpuavcrfm.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gsyroqzcz.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gaxlygnkw.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gogendrpk.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gesjvaksw.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gqyiajith.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glpwwxwlm.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gojpflwsr.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/glgwfmhpu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gbesxrgxj.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gywgjxkss.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gpquklovm.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gtocogmvp.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gzaadyrlf.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gpjbydjnv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/giahvupvx.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gdouqyowg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/grjmmxtor.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gfqomwuta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gpngcahxy.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gpmouzujg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gmlwgfvpc.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gspggoorr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gitakbmod.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gavsdroht.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gaxwiyedt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gsmioganq.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzgapqdbx.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gpfbfrdle.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gglxtpyuh.sHtML


<!-- 参考信息 -->