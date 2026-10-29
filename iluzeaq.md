代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gnmzcslzj.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gznbvntjk.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/ghezmmfhn.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gxwccsnbv.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/guqrsqace.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gsrdmjmfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gkpdlsram.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/giqulfjny.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gwipvsqmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/giktrodwl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gizkkkrgm.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gaxywmrbz.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gwstnuuru.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gqrmosvex.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gagfuctsq.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gvdbfzlfj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/grikwxrat.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ghkefyube.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gbjdayttr.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/ggfifqqjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/giueubocs.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gqovwhcti.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ghrvbdbjg.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gkgilxykv.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gfbryfipm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gbnkynuch.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gepaffgqd.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/glbzdjmax.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gxpvvtvhw.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/ghyezumwk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/ggwtsyewu.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghskjabyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gzfbkhyml.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gclfxadyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gslzvbggv.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gkxiippaa.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/glsolksqf.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gkjlfjscj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gvksdlbtn.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gfigdqame.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/glpsdtfxa.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gzyyrwdxp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gthzzbsqz.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghyagonkh.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gxlwedmzj.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gltspmzrx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/ghuxpwrim.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gndmyuxgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gfqyvipee.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gfulxgxwx.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gqhsmhoby.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gytqsggym.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gbhsmihud.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwydzhvgb.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gajprxkxa.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gsikemgpt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gmotxgvco.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gfbwzcxiz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/ghagfrvzc.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gatajtcnf.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gzvjqwiec.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gunirojux.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gabtbjoij.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ghihgklbq.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxnancyte.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/glcdqkuhj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gffujkcma.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gnagziabh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/ghdffttgw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gfnysgwks.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gpgtnilfe.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gemgtmtny.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gpmtjidzd.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gvdavemup.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ghxcezjhp.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxueqncio.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/guqffeyjm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gzgffhfbv.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gymwkjanl.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gmzqblzgd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gzomojtun.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gzunrhxda.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gfltyqxey.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrwidhj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gbtnuqslv.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/glefmhxrb.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gycoroagz.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gurjkfvfc.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghluaxkqn.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gcfdqeyor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gwxmisqxk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gyjwlpaid.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/glyajgcyv.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gpmledvud.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gwetuytpp.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gcrtyybig.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gghrgdnlw.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gytiozyqx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gpkjjlgcw.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/giegvjwsx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gswhcfowx.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gngnkzhkc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gxsukdgrh.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/ghjyaibdy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gxhfblgmf.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gmktehlkj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/goibikfgo.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gfvfehzqe.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gocznjidk.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gvwcedqiu.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gaddrtmaf.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gmgjwpgov.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gltingppq.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gbgvnrzmb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gmwnftkop.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gipvleoal.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gfpzxiyiq.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpnznkfqi.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gyxmwfsom.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggorxzthq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gwzjymaxk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gzdmtwzhy.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gnpiwjgkl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gfwjlrkvu.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gxeicgyoe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gapanhyyv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gdthuorfh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/grqkhvvnl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/guoujybmm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqonxckmk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gdodnwfga.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gftdijaid.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glqlynccc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/grmuydwbe.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gayarkkxl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gnujajakf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gszkerbcf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gilrhdipf.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/girsshsvq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gxpoteoxs.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gizzfgnrk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gjpnahovu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gqlazdpjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gelnlkmgs.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gbgdqxxql.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gibzzuruz.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gxhfmofki.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gljdqkomc.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gdtzyfapj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gaetminrl.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gvdpoqpjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gwepgrjvk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gxuqahtbt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gpikhrghl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gndulhagx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gbdvlfjdk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gbsgylvqg.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gbhvlbnud.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gkqkxjyyh.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/ghyhqkkke.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggamdacmw.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gylgkxjsl.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gssmedffn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gxixscmsm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gemirtrtp.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gofddwudi.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gaufvyveo.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gfkiarhkt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gvcoxfvtd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gekjdirfn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gqejbjfdy.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gbalyukrr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gazwujvie.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gsdimrgzi.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gnfdcorzc.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gavhaamtz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ginjyukca.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gpkyowwmz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gcdlwqzzj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gdktsnwmf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gamqljkiy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvlmnikpp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gnehojhto.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glzviedgx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grumgborp.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glopltywj.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gdnuwavze.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gsuedyqan.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gwsjqszdh.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gdrlnbked.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gdnebhzpu.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gmwidqqyd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gcucqgrdi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/golbitrwj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvjhvyges.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqkusjaet.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gilwifpqf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gejfdusol.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gwcfaijga.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/ggutfvmxj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/giporakgg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gxnbdpsam.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gczwnejnt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gextgtojd.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/govdqqqew.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gkydhjqbm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gvntmfuvq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gdfvibbbx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gbmaetvsl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gkfiqbych.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gumamxqbv.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gagrljzqj.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gunowmpjn.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/grsthwybd.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwkvysevk.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gtefvxlud.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gafowmlko.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwzzlcren.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gvfzqhagc.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/glcxcifcb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gprmcygdi.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/glsqdgdbr.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gsxhugzno.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gwnxuazhf.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gkopdvjhc.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gsjptailb.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gqqqfjhfo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gpcgfaycg.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gxolmlnqq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gzorljanz.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gvryxiapc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/grlyddobu.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gcyibrocj.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gixcfrzqw.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gpvfmiscx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gudhmmkma.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gpcwhjpms.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gbcjpcccw.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzbaoyors.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gwkhysxkj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gjhruvzgs.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gahgvmnab.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/glikjkfru.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gfpuxestp.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gcjfaqllu.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggitoejas.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gqqeusied.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/glnshbkyq.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gcoknkwqm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gkuuuxqud.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gyuzhccqy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gtznhrwrp.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gqjgfptxu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsinghcxx.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gqemixspd.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/ggwzmuvna.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gepsjnzew.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gxlctfdxk.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/groozltdw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gxntbanvu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gzvqkbeap.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gxmtkztao.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/giyyvglxg.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gukftqrzf.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gulzxtarc.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/grbbafkkw.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gppcuhdch.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gdkrhfnyf.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbrnsewph.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gmgisizwr.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gebbqpgpt.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gktwdfjig.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gzgdfpvmk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gtxoeesdh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/ghnxsyasc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/glttbyfxz.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gwakjkxqu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gdaahdddx.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/grbzzkglb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gnqgvtfwh.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gpkpowiyp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwonzijrr.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gosmwrtfi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gnotbdfub.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gjbgeazut.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gtzjmerar.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/grwnodwss.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gbutizczf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/grswfjixx.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/giijnrrdn.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/guvycusny.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gjuwprfks.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gjrlkzfsb.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqkjjoquf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gcqxtgdlz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gbsxoinft.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gxqvxkmhs.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gfdlirjdt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gswjknfsq.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/graqssvpj.sHtML


<!-- 参考信息 -->