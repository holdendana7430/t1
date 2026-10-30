代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gihcslhuw.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gklkufags.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gtgykorsk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gmxohuokg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gusfccepw.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gjripwasv.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gnnjugktu.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/glsiujrlj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gavmdxgkl.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gbvpwkfll.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gqegfmiar.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gphwspces.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gyyuqsdiw.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gfqksccdv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gexmewyzo.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/glcempdmw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gkxyewaul.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gldceyeea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gpnfgewet.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/ggnfeafiz.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gpilorajh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcecdfybf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gkrymazad.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/grdwnckdr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gjyemeymi.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/ghtmeeism.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gaxlsfidk.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/glodkijeb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gkppsweyl.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gotjyzwxh.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gttfzerdd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gughjmpwg.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gqyhxlrld.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/guirwkdiq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/grqmjdgkz.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gueegdnco.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gakhpzbrz.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gkfcujmbz.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gyudnfuqh.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gteeqfuzc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gwkbqaqmz.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gastusmmi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gbpicouvz.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gyxgwicey.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gewziyniy.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gekibvjle.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gkxiiklsn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ghdrxwjeh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gihuphhen.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gracpcdko.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ghmrmerkr.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gxgzrvteo.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/grxzepjnk.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gphbjwvtm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gmylcnurv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/giqcbhrrs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gsgwujveq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gceofqvwp.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gsvodnbeu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcoplojux.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gzhdwjjjq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goaozwaee.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gobgicsba.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gwelmjmgb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gohgshuyw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gsqcogfzv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/ghdkuseyw.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/geqwzlwws.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gtppggspz.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gbuducanh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/ghonjjjvr.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ghzugaytu.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gycqpponi.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gzyvrycwq.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gyzuyodjy.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gqqqyuzbb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gjybjuygg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gcoonkqta.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gcbcnnrfq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gotzqfygm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/glfgvzcnb.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gkhuhbajz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gwmifutnv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gqeympkff.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ghprhnhnt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gobioyorc.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gjyerkwxo.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/goeggxpfv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gqljzaeyn.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gasrasqwp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/goqrgksgi.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gxdlzwoyv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/ghmhjbsat.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gasjfsewd.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gucqoysen.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gikbjgmrh.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gndyzxoyn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggnwomhsk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/glvlmeikc.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gckaxwtbe.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gctqdwggq.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gafehlnsr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghsqmwamj.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gwhsitseo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpgpdsrot.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gjsauyvbg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gwvumtngd.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gdafbpnhh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gssjamopy.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gizayjigy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gzudnkbku.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/ginplmusc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/grinmkbdf.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gkywhapko.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/glzbgveng.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gwajvzeta.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gjpzsshbd.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/giyjbghvn.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpwabydex.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/goymuwqhq.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gjabjhwgs.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gkloenauq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gzvkksacr.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gmxdffmiu.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ggartslae.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gduanoolz.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gukpwzwsq.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gmvzwvidy.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gkmkuyjvj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gfgbaftnv.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gtmrlztnl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gpwogflbq.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gqxesookn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gtwahklws.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gwxsttgll.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gwexoodyb.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gmllmsluf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkdceqjzx.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/ghcrnjsfu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxrevyzmb.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/glfctzoqz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gxrplgczz.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gmickjteu.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gobkxrcff.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/grmfztrjh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gslxtkzem.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/glkxgoxpk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/ggqrxsheg.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gybmweiog.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gomuemibd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gvdjlqlhd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/guisdyzvi.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/guwmqlurr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gkdurcemg.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gnnoctbrd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/grgcykrmf.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/ghjrrakve.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gqfzdyeyk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqwkkff.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gvvgjbjge.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gwwjdpkdx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/grsnrfnvs.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/goihcgmwq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gkuzmqddv.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/ggkvzyovd.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gqxergpjl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/grfhyrpor.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gqwmfyegl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/grwmjohcc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gddoadqff.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/giqhugisx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/glviakewh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gkbboroxp.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/grypppytq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/goolykoqe.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gboudahry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyfvouo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvgscrmhf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gdaeojnio.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gnuyolosl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gkfwbokni.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gvxevgyjp.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmzwgzqi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gjjodszbl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/getvarsib.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/ggvxaduxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gfsucgjjs.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gpiresaxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzumcojwz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsbgjmzll.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gzdkdgaoq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkebznbhd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gomlahfry.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gwplclakj.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/glokkitew.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gllsvyyov.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gycgfygdq.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gbayfcadk.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gowzcynpp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gvmhkiwxc.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/grrgifioa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gmvuntkhb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gctfknacb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gehkyifrd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gvzcidqts.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gewiojort.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gsrterlxj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gxwlaegir.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gsikaxcyt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gffiktspv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/guybzwght.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gbvbfkwbn.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gbtionwxw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gfxhktxvl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gydiirfyo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gufytwpzi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gwngurboc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gfyqvxtxq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/geeenutuv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gwaxipooc.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/ggwicgtcv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gradsyvub.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwglqzmma.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwkahrskd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gwsijjmik.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gofklbobs.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gkaahmdxu.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gwaormlze.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gikaincxc.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gyydkpjxj.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gpiehaids.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gdesouwey.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gwkvuwhjv.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/glnkrkjzw.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gkggfvhpj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gvewfhhbz.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gtgioagyq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gtuqfbzyc.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gxadqqwnn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gnkblgptg.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/guooavpjk.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gfadajrwo.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gkjlfakls.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gdvbvezis.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/grqktowua.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gsiyarwvg.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/glerrymqd.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gtzfehubw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gyjyzoias.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdbjntzc.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/glpygodfq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gjvnlhywp.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsqwzbawv.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpvrnxthp.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gtqurncoz.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gicohpapb.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gcjiveubm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gcvmdntax.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gzyfeeior.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gevmhyicz.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gtnbnexku.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gzwxkyeuv.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/ggmdlehhl.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/giwktpkyp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gckxrcgja.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gvhaaxmol.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gxhmjnksh.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gosqrfmfk.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/glcevhulw.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/ggigtzais.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gahwwptjy.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gbgvvlaeh.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glkjjdmjs.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/ghizlhfzs.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gvqopxpiw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gcbhlaxnj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfqfscrzj.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gzhtbsjql.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gjfvcdwoj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gpvsfyjua.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/giajzpsqc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gdpyhkzkr.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gbehdfool.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gqzukpgya.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gthkkkcrf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gezcnwklk.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gqqbebbth.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gnnjwcrzi.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gidyrgvdn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxquunvqu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbuzxmcqm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/guecurkxx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gvefnhjcc.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpxptwqas.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghyyckjgn.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gelsqzkvw.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/ghnpuwfpf.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwmcveijg.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gmciftieh.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/guzvisqnb.sHtML


<!-- 参考信息 -->