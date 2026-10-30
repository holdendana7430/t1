代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gxqckomlo.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gfidepxrs.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gamvjovoh.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gkvpiccxp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gsovohdsb.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gernvptvf.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gbtgacwen.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gdgijdnzu.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gdbtavujs.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gniyafaym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/grlqkevwo.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gedvsvmfr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gguvkfaji.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gjfrrichh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gxmcucggs.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gtxlqmwaf.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/grvlbqaqk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gwhyklvjo.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gamwamjue.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gpacaldai.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gtpjdzyuy.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gtttcllhs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gyuajefbs.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/ggwcfbwpm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/grapfnzto.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwwilcqcz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gadawfxeu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gapefcgkd.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gwrwkrztt.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gcdsibpbz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/glseqiyyy.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gqurzjnza.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gdagotnci.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gkljtzhou.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gjzngbrez.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gcxmlkote.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/ggngbqsth.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gepdkoehl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gsxexhrkb.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gwbhairwo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gamxcqzoa.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gwmiknobm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gzqebyvti.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gstapjejj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gflxsoecy.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gfhkridij.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ghswgtuhe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbqdaka.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/glgqrfred.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gabuyzslk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gventjahv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gftfrfnun.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/glhcaxydk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gbinfjyoc.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gigpcjhhm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gobsitvuv.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gvtyfzlus.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyrsulpdb.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyyvvfiwl.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gvhkmulst.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gtxuplmsg.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ggykxfqja.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gibcjxiqi.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gitptipps.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gegjpsdoq.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gktvbbpio.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gayauhktn.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gaptrmzgy.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpogcuyl.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gzngayywu.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gwkkaouso.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/ghdscrpgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gfxgodvrn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/ggftrrunh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gnabeyree.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gzluhispk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gblezrlvp.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gmauqqaqj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gcdemfaaq.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/guyckqguj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/ghylbmjpi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gkrlvivhz.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gsenffbcv.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gsftapkbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gplcfwjlr.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gsntamubo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/ghcsnzlnu.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gmrgdtyka.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gkhsdyfpm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gmbaniumx.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gxtgrvkcg.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/giveimwqc.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gdrkfqwwx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gznhizipx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gtfusrsst.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gynczihah.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gbjpcfhqo.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gkczigelt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqhkfchla.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gnuwzahbf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gaemrmrjz.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gdmbtvqga.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gkmeblooj.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gqjqnilfs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gvmqlnapz.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gkhyvcdrq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/ggfhsekme.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/grbksjuyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gtbszuwzq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gucekqegg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gtsqbpedb.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gbgbintdw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gfouhflxi.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gglppblot.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpiexvehk.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gqmwrptxw.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gmgippxat.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gfalkfgba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/glveznxxh.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gcpxkgwxk.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gvdzxzxmx.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gvucvtuea.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/glzwovuwe.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gksinoskl.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gejyegknr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gahktjhlw.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gmwrfjxin.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gyzawxxar.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gjjrcokkc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gvmiiqcyk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/ggmkyydux.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gyspjoyxq.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/grsmpsflv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxjtvlapx.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/grkmalauy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gucyhyanw.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gtaqwevjv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gpabglhkm.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gblvhktxk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqtaamekl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gqzzyactm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gvbugchfr.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gingpjaeu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gtpjcbmqt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gxxqvfupy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gcnrqcabp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gytrdzute.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/glqgsmerc.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gxhmovpyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/glcccwysm.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gjdyrhswn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gsbbamucd.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/geweqvise.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gmkymlfrw.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/grdqqemmm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gasxzuanc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gnwnccygk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gvzamzmjc.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gptkmskow.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/goyiqisbm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gfchyegbw.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsghrftmi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gehwqmivn.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gbeghlwoq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grqnljhsx.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gurmjtemr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/getobjfgh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gawexvsos.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gluuapewx.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/givmsvrsu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/guafzlzea.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/giwwbvjud.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/geiepbque.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ghajrnaph.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gumwmxoip.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gvhtqzjzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gkjvqxbps.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gkwhlaqgg.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gejdhztak.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gcyrcjgng.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gjkyfkhkx.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/guoodhmzx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/goseuhmoz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gxpvomooo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gzduoqdrk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkxgoiodv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/glniewzob.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxaabgnmt.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gbdncgxlc.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gfmfijoak.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gnhgnzdhy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gwhpmkygn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gfrzurnng.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gqamodmsm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gddzvdulp.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gmsnokxel.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gtyjfmxht.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gljnuvphs.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gkitqdgrr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gbdbulfcq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gxwyotafl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/goapdmuoh.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/giwhveqpu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gybflrbbq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gjcwjjfea.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/geowtshzh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gsnpbwxsy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/ginfklwvy.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/ggxrsbuub.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/ghbedvkbq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/glnwitdry.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfegrtiek.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gkzlojdje.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gyeuqehoc.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gkimrshzy.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/glxcdrhfe.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gvhkvetaq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gkludmdsi.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghdavosbk.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gkzsqjrrd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gjwfircbc.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gktpctuya.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gznqhzamc.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/geutusmnr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gjruzzehg.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gkznmdojx.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gncodonpf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gjpdwlurk.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gnpoiprbi.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gqxtthhml.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gwntncacw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gvzyncstr.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gjpubntog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gpzsfuqph.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/getynagvp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvhbqmt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gtwxgnnhd.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gvkkdqofj.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gdpypkjwz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/goaniecqr.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gsnbdjdvx.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gpyspoekh.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/ganmfgstt.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gvaqssipi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwyvkeviv.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gpqohvhol.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gzcnjbszl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/growsfpqb.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gqqfxucjs.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnlusygjl.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gxnjibisd.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gevspucqd.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gvjdqqxqw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gajltrqez.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/grboovmjr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/glwyjxpcg.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gvjsyxvqv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gryseznwl.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gscubgvyp.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gakumklxx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gyxxolkvb.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gvyeycjkp.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gzctdpfna.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gcrrzvcbl.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkugzhcgw.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/ghtfsnhme.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gdxsuydwi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gnxwsjfoy.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/glxouvdfz.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gcigognrh.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gsdzrwymd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gwsmmryly.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gmarkfrqu.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gafvviqtf.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gaazubiia.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gizwwbfsu.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gcexsaujg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gmbdjlufz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gunwflywu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gwkqysnrq.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/glrsxkazh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gupxmkpur.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gbgomfrgu.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gupsuupms.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gamizkfnb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/grshzfsqu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gddpairog.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gnpawwsrs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnptdee.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gftzixmzf.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmcwliyqf.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gyvswmvaz.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gscdqyrkf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcjsrtrzq.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gkgjveodi.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ggwsfebjh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gtfchkhcd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gecipoklk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gasixahfh.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gyknqrtnz.sHtML


<!-- 参考信息 -->