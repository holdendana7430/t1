代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gvlgvkvuj.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gvefjjxlg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gdfhszhhg.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gtnlfashh.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gifbmqbmh.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gfzpcvthi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gogwnprgz.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gaxwbmnqx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gsvgvpthf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gyheljmct.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gxshgrlod.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gbgmgvmfj.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gaftlzqjy.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gcmpvigry.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/goxuvwsrf.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/geaetrjkn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gwbcipwxf.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gjyzloaae.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gxzwigcmb.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gcbljjgou.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gcqajivlk.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gqbdulejz.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gcnmaumrc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gufceqhtq.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gfkaibzby.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ghdlticlc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gyqvqxjig.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gundowpjf.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/grcoiavae.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/giikzctso.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gglunstln.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gdbchdqqo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gasjzrgxm.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gjawehzgh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gcbxrwvmz.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gwsgrqldl.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gpfpbzqpf.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gkrwfcler.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gnpdvemnz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gqikuscnt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gdpuqfcfv.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gmeliosoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gkhqsilhj.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gnfjfksrl.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gaocqlpiu.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gbwlyyukx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gvzyxwyax.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/giojrrjlc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/grhhmaazn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gkpdpowuk.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gdoacdqvu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggpnibsvm.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gnzlfpjnt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfuycwgkw.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcgcltaqm.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/grdbvbiyi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gtleozlre.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gjyfbgwww.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gpcwzbyjs.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gsvsjttgi.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gzdjxrygz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gfzkmjhod.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gopnguzcu.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gzwcupujv.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gqhiexqgo.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gnnnxqeom.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/goicrtvnq.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gsejburjv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gdzvzftnv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/giatuqhiy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gkpywedjj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/ghvloxkss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/goigmmbve.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gmuplggnb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gszhaplfp.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gnmgwtbbi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gcxbkzcus.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/geottuhra.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmttili.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gawpvigdb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxvtyioxp.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gbxhivniu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gaxntjqac.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gcdcycymv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gralylprf.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gvnwqspcv.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gyeaufykq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/grjzkikei.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gylzdmces.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqrewuysl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gufsptibv.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grrasikba.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gajfabejc.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/ggsabwpqq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gnpcrcpom.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gojxpvmdr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzgctkvrp.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gulreqgqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gjhtwtdpp.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gihehcsin.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gziqgdbov.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gbtatkqrk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gotajgamj.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gegzhohxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/ggxwankvw.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/glxiiuygz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gjnovvetr.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/ghvyqdrko.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gpconxtkh.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/ggnkthgoc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gvgpawrqb.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gswbzwypf.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gbiosgvzk.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/getayfgct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gpnkfbkvt.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gfrvhjizw.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gpcjwvvft.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gcjqzrozx.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gcumgseia.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gofayshfz.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gykbbulkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gqaozexux.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gtbaleokq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gmrdlkkcv.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gzxunflon.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gptzewptx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/ghhinvezm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gdomdnlho.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gyunudckg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/grwonbzgf.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gwdikexwz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwoocvqln.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/goplabmqn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/giiazmdku.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gushyuiha.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ggjlvgypo.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/glquanljh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gcevvmhmz.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gnqfwzkdu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxdogzbxx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gedhxiebs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gzwvocmta.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/grpjvmjoy.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gdcpznioi.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gdilmupsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gqzjipqfx.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/ggfzkwaju.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/ganlnjeyc.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gkocrxzcu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gogehyzck.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gcprbbxpr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gvkdsbmpi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gggdllkdc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/genrqtktx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glusgnmxq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gkmutvmgi.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/ghhakdafu.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gbagbwmwt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmabrrpki.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gyjnyxlhe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbcnuydzn.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/guqhwbtsv.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gagiykevf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gxdvovsaz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gjqvpyubr.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/goxfezaoj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gpdgftprp.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/girutfith.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gikwqodhl.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghrfogzrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkdtmljvu.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gsygbzgzj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gzfdrulbi.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gtwotreim.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqsmstqqg.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/ghhzformi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gfyiafpsx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gmavipayk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/glkzotycy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gckjtqbkb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzkxzpdba.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gphynnchn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gzsuseixj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtbagcfbf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gztmvholw.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzndsxdly.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gwpdmsuzl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gwelcbkpn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gxyualqwb.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gcxascnty.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gipmactfn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/ggqgotimm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gyeaegvkr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gizsnavkq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/glcpbicnk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gbmtievxr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gblxxodiu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/guwnuaqsh.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gvljacayu.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gyqhnleqx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gnuicaddy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxpoqtayo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gmteebiur.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gjvpglini.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gprovoqtw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gbkambeah.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gkljesryr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxkmruiel.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gizyadkzv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/goxsaapev.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gsnjowvdc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gudsrmweq.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gkfhlrymp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gkqnfibmt.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsbbargff.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gownldcor.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gczahvqzh.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/goqqnujlc.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/grtngkcrj.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gxtdcomjv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdxvyfzod.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/glsrnouig.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gylnjjrdk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gwmommmvz.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gzotdkeax.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gszhrptqv.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gibbdivbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gadldqhsl.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/ghbcxhfiw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gunqvcbhx.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/grjcvvuaj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghmlpxrvd.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gvaddacdp.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gjojlokou.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gjuysgkvr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gsgjlrxie.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gxommamnz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gcbrnxpsv.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/grdufhbte.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gqcenmhfp.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gjxiaszpg.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gtwkjranr.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gsjdgftwf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gbhqefacj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gswuklbqz.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gsfftfamz.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gjflywrrj.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gqpnnxgzy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvhgaua.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/grexrfekc.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gmfwkpigb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gzpizieil.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gosaukvug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxyfebtaj.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gokfhdnrv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/guzfwmpsm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gxjaovyid.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gawciaeak.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gnsbfefui.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gqflwgmzr.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/grhhmaxpq.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gerhjkppa.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gbtpcorwu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gzzxcqfxw.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glgrikpzj.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/giqeronvj.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gcuxqolvd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ggxszuoty.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdqzqzgms.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gdmaffntk.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gukfvswwi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqvenvvff.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gdhnytatj.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gshxiarqx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/ggqsebydt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gqizhecgx.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gkihlprrd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gylytkzyz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/giqlecpps.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gslqgmtuf.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gmmrdykjq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ggyjhbkzy.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwmmasycl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gnldylegu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/glmuxsyiw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsgwxtqch.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gzthdnepw.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gvlmvdwph.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gbtcfzfgz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyomqqxbp.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gxixhpspj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gvtuygbnc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gwukluems.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/ggxzpiyed.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gjzgbqubl.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gblzkcbbb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gputtbdak.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gkscrwvea.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gerglgrge.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gjemhegcq.sHtML


<!-- 参考信息 -->