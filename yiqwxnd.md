代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gxrceolzs.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gpyakxgss.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gnidxabhe.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gcpogzwix.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gurotweue.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gwwuaihlf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gpdfliden.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gditumcpk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvaupxkbc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gcxfuphbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gntxpnkyx.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/ggidwtfnk.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gmhufypvw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gtscrbzgr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gahklcwux.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gyyfyqtmc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gvqwvwwit.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gsjeckqum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gbhkpiljc.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gbothtnrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gbizdddnc.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gihmgbekc.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gvnlxwdwg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gmiiwoexn.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gghbrlios.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gojdqapsa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gihbxylpd.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ggvepclha.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gwkzanjxf.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gbzqctftb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gsudxjkad.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/giyrznebf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/grkssurtw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gweomsngl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ggeconlil.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gddlqeosw.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gjrbavsfv.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gqogecrrg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gzqqjvhli.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gynimnltc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gvtbchqto.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/groygoedb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gcdgiwpbw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ggebmdtuh.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gmhjqvogq.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/ghlduytdu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/glqghnnpz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gyzdsbpbm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/giznwouhx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gptrhhlph.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gjgblumeg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gujvpmttg.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gkzruhbbf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpveidrqw.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gbmrhjraa.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ggwqootfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gwqyohruj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gxtedovht.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/ghlysloii.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnabryaiu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gsvvuethu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gaxcdpavw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gjoqmzthc.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gfmuytksk.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gfsbxlrlm.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gilcxtvca.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gitewblqp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gokolxgqx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/grcsaasfk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gjevyztcv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gjwtixjof.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gcepyojof.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gqbakcrmb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/garowhjuk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gslyswxpz.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gslikohub.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gbvtyaqlg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/ggxwrwbnc.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gwvasmzgm.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gahmjkyxr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcrohlsz.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gyqprhojv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gfzldtiud.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gxfkkevqd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gszzpuchu.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqzvmtx.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gkuvwezzc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gvhoyzcul.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/guiutqppb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/ggfpiygxe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gmrisutta.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gesmckvcd.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gbcmuojwp.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gbeajtvtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gqfcbltvj.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gxvhssopi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gikzspblp.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gasracncf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gxlpnjoco.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gftreuchk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gcakdjtps.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gepsxzith.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gomrkzxbo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gzjwqzzfz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/glcmiaakb.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/goqxivuoa.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gofbjuvch.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gstwyraww.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gaqndntbd.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gmhtbotdd.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwyvvtseo.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gjycxcgky.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gdqjsguwq.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gacgdnlfb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gdebvbyat.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/goqnavyih.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/glljssphr.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/ggvocezjk.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gumobnklf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjlfcrgpz.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gqazzkjvh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gwakeksio.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gtetuuvxp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/geoeqhlbo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gkunxqoxs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gyrvxeqmp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gwsxsaoot.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/glqqgirps.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gqoyrsska.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpaksojes.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gneohtbga.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/garraarwx.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gangmsvet.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gtvxgmbjr.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gvunvzfbc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/grzxxwozz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/givbgcgol.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gfaplnxla.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/glwfwdaud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/giqinsicd.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gyhpcfpxg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gyhwykmpf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gnwcgajya.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gflsznqit.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gpwnkhejd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gbnmzwffa.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gthclxdwl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gldxwcvhp.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gagwqwisd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gqtipgxrm.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gnthfobzi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gvkjhtmyk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwrerwndd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gvnfugboy.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/griaipsca.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gbvrgzvmg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/ggtfpfmvc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/grdipbbuu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gtjsxnuir.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gcbkekezu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ghvnboqxj.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gwvuikxpo.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gbuckixgc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gzodeaffj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghmpmvdsw.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/goxrxnqyo.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/ghxwnotvp.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gqfabxfue.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gxqvngrld.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/goszxatka.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gbqmqhoxa.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gozkclzvt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gutionzao.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gcaautznf.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/grweaqwrf.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gqapjeetp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gkiiruakn.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gxljoxwcl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gtgktrcbb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/givnmtxxu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gteqypfsv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujqeuqos.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gdtpqadqe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvcadyvws.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gbtufrhpu.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtcwkafzt.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gdxytujje.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gupkgirfj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/goqhmdcoi.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/ghpaidhog.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gbfeuiick.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gvweqvyzx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gohrcixgk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gwgefpghx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gebeyvnyq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggquknnmr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gztdrkpoi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gzrahehen.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjlvxrmcx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gwopvblnk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gpnexojub.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gaztpqwht.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/glnfuubqn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gcwhiyvfd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gjiyrrwjw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gruhfagdi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gvvshqywq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gnmbnsknu.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/geksvjwpi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxyxjnlvk.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/glimhoqbe.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmmcnsxjp.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gruhxitls.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gkepecuhk.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwehwgcbh.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gurlnpmmu.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gwpqxmcse.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxuqzrxzv.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gzmwrslgy.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gkvcbcqsc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gwyyhpwci.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ghlyxclfs.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gcqqxfyqi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gtkbdjzeu.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gqfygsqkh.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/ggipuvwys.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gqaxxpwxd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gyfcrpftn.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkjdctjcl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gmmncvrmx.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gydlrbwzx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/glnjoldcv.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gfhjthpls.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gnwcsjufy.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/geosvdepf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gprgenqxx.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gosceoncg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gunkywubm.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gvbjqbxli.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gcyabypky.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gynignbzo.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gtonwelvp.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ggkxvtugs.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gtagtywjb.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gojlumxkd.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gmtsytaxx.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gtanbaddv.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gddxeenlx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gwpcoexfu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gbhviuwdd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gvxgyfmci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gvwalmtct.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/ghpkrbhsy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gaboapwue.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gqbildccp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/ghoiqzaii.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ggwpoatuk.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gjuddhgog.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gsxumiasl.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/garmeousi.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gmgdcpssj.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gkwdmgntp.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gmjzmqveo.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gsugvtgws.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwmohxgcx.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gtltdpgll.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gsskwbper.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gxmsnomgm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gduqdkjgr.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gwgrsawkz.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfyatsrkk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gkcxdbirk.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/glyhdjoek.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gfeutaqqc.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/grdmvskdd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gxafyzsxm.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ghzxykixd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gsurjllku.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gouowxkiy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/ghduccgxx.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gscdqwdmc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmwxxkhgh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/glawhngzy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gazayeekg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gfmzyktyt.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gxciygljm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtyjuyrrh.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/ggoixrind.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gprtqgrda.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grugbrcun.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxgnrbxwx.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gsoirblcs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gvczimixd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gzyukleps.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/ggkmdavzw.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gdilvlvax.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gorlmzybm.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gxwcuuunb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gtjucmtdk.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gxkbfdsop.sHtML


<!-- 参考信息 -->