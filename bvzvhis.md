代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gtugjgokj.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/glovfrpsp.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gfqsqcaeu.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gewgekdvc.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gdmvpmvvo.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/glfelzliu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gnmpbpjkv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqsiauqfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/grxbtlnvi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gttazisuf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gwuvqdyoe.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gdpzxzhjz.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gopugmmbv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gsqdjqqdi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gfdhoeyra.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gxitutesn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gvyydbfjl.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gglvcdduk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gitqezboi.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gakjejpzy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gntspnubd.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gciioifts.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gtynzapot.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gamwtxsga.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gjuwejyen.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gkwnoeymx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzvvjmbbf.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gpsgotubw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gsxinyhwm.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gsrgbebyw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gnylevatt.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gzuxucmsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gzeqecafp.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gevogkgzl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gnumskfvw.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/glaenitnk.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gedpmeayk.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gttmindgr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gycdpwxga.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gugcowjal.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gwjbkmmpw.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gbtajdvos.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gvwwchnaa.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/grscedmfw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gwemutmvp.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gbiypoirp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/ghjpegcff.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gwzrfeumm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gdcxvxjap.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gxgvwrytf.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gdypxakld.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzimqzjuu.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gbjbcnjmd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnkidmeft.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gyjgbafmf.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gcnxouemu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gucizrojg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/ggrjmgxvt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gpoyaftoz.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gwzcemtnp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gfweexczk.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gjghvrxrj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtbmmeyky.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gcliyvxnv.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gkxzajghy.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/geerqipdi.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gjyojyhsv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gcvioadgb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/galicvzof.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gytyzflcq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/ggovevqko.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/grjapqpkl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gwcvayfmg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gnkbdjqzg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gifwtlwia.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gghebcbqx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gxsffxxgj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gqebgqijk.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gkwbnyhrz.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gnuatqryo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqvxgksiz.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/ggbovrryx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/grdprwjjm.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gvetmgvqm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gnwtpiojj.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gztdwfdox.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gmhbhuyxe.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gzemwsxct.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gatsdedaw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gohqqpaeg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgboomeb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gzkjymkae.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gdpqwlres.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gfegakvwk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/geiixqpqr.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/ghambfddl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/grfyqbxrq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gxxoyhnyf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gdtdfjrmb.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/goinrazun.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gomnomjeu.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/ggcxruqdw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gwlracgzw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gisqxnqkf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gflhwmzdq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gbiqveewb.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzuvwsjmw.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gilalvjpm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gmdxfyujs.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gvymtblhg.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gfaurgfxl.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gpvisfcba.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/grhlxucdf.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gudrrtnpo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmlyhyrct.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gaydwsvcf.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gbjxcgccx.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gderoftxw.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ghppmhvtq.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsytbscey.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gzvgfugkk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/guytsaugp.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gqenxnozn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gowpobejw.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/glmaypmzb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gwuepidku.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwicembct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gtxcstlqh.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gvhbhivls.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grunehwux.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gxykndfae.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsepljdcb.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/goqyltfvp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwbojwef.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/ghnyohhkx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gligayseq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gbyrzvqfr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gwmpllhvz.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gjiprukht.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gbuuhmizr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/genwoxdqf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/glsgvujic.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gucoxonsy.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gujrtxyeo.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gazzkiwex.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gagruluxn.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/ghrppbzjb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gshejltqd.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gbinfkrxq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gxpxevgfw.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gntfjokvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/guymfgart.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gtseeifwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gtwrehint.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ghgkpiuod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gqapopauy.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gfspvtikw.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gjlbsannl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gmqgocwbe.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gwxvcsmmh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzqypslvy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gwlpgooee.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gzvijglwu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/glxleumet.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gardyvvfv.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gdvdqudyh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gggmsoqff.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gjgnzbqwc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gihzwuteu.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gjcxdfyxv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/goeuwhubq.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gzjjoslev.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gymhynysu.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gmupsqogu.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/giftxfopv.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/glgfvwbou.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gzdqoomaa.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/genawmixc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gtyxedzon.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gkzeesiry.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbzjrocnv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glvbyqatq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gbxnjfpbq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyzdqnpyl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghuyqtgon.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gyvityvjm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gakostacp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gjkdanexq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gldlqmuyj.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gfymfpcut.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzthwkw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvlvpbsul.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gplozmavk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gfwcdwjpj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gmwwnkxus.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gnjzmuwkx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/ghmtehptp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gnamqjgzo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gfuberumc.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gdhiyjlol.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/ggrfrjaau.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/ggdkqrgcq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gcuoffjyl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gkxfedtec.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/guvrcbhie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gulmdwbee.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gltlfugzg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gzyhxppkn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/grwcqxoac.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gqidtnlck.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gepobgvic.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gopedstjx.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gioozfrgk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gntiesajm.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gumwkicoe.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/grfcklhbr.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gqbnnwvbh.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/ghldangku.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gtiryshej.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gmxsryrnz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gyekuoven.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gopdridol.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gazfwsukd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gertuglzp.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/guiuueink.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gmvtbwowy.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gfaeopvfl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/glbfxcqbc.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gakxwsdmf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/guoyqnbcv.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gpmmywtnb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gzamhrrig.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gbstybhfg.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/guweioihl.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/glxadwncv.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gtjhtbktz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gwabgeowm.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gfgbaxjef.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gzuijrrus.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/ghjohfobw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gdgvcwqnz.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gombaewct.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gwrepdmxv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gvcbopygo.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjyzilpax.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfaszoxti.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gybmnyexl.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/grmfwzmyv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/ggyanpcgc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gxyhnioqr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gitwoocct.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gmxydbdlj.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gzijlqsrw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gnzcksixp.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbzpzylhn.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gqtzqpsgg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gmofcgxaa.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gbazgpuhe.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gfpoztgzt.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gnvpqufow.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gjsmapcpy.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gfmwwwczj.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gdtneznwm.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gyfaoiigh.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghuwuiwrf.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gvoodcooa.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gsqrksdyo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gbwhwhbhk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/geznrhtae.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gbnheawme.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/ggjqiwvuh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gdkmnrdmj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/godnvykar.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gaahpvarj.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gcojypoqi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gyqpqtles.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gobykoyrw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gtszeubgb.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gyjcgikhk.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gaehxrloj.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gbwucjzfx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gdlypuzzx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gavpfsdgo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gvxyrejji.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gythayvmj.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqjphqalf.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gwfhmtlos.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/grigstuoq.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gedizmxuc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gevgmxaxx.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/ggjdpuskb.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gcfqyxmhc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gmtfxvnqh.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gukcpgkhs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gctcanvyq.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gcoifqwws.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gkcweopjb.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gjulwrxah.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gfmwdteem.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gakuvytts.sHtML


<!-- 参考信息 -->