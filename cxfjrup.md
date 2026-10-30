代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gvgmpwxqb.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gionocqcz.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gmtkcwhpt.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gvstfjnyq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqlyswrli.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/godaiyldr.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gwybfesky.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gbsxupqvb.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gacftmbvl.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gabtwzjjr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gyrptizqp.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gotrqqkzg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gqlwlwyks.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ghkghzwxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gmuwkqprd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/glmxwhozd.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/guvjfmvyy.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/guzcpjpct.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gmzuxspit.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gaxubqlii.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/ghpjksizt.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/grsbxzsjq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gxcoliuof.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gewcljagl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gswhwnkho.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxngtiyor.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gimqwtjqg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/geuvvkqfp.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/geuulmice.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/ghtwrewlw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gjsxcsmfa.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gihyhheak.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/guczhjlmf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gihcqrino.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gazdshamf.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gzegmazwf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gtzaxvmvv.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gtvmzshnj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gvyyqubsn.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gknnwlloc.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gidnduovr.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gvwwsiouj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gejxbozwp.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcachutvl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gcpyxaajj.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gvizvavfx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gokowixsi.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gptgkjooq.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gfcrhhmby.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ggspupckr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gfqrsucvd.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gxkurvzyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gsaoigpvg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gmaaexucu.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gfekxlrbx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glbkpasck.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gwmvaoyyj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwnavxxfp.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpdtaumiv.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gouadenxf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gzsdvwrai.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gxxnhgqwj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gnssxzipa.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gbqgtpbns.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gtwogzubk.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gyjdunkgr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gntsnqzca.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gifvbtpzm.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gdmrqmqft.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/ghegzfvgf.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gdejkefcy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gvuwumfpb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gfspwujxj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gruwdabev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/geesapudy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gnqdpxtzc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gaumicoll.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gvixfsyzz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gcfusnawj.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxtthwkbt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gqqtmkbzs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gglgbhpsr.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gajhxqift.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gtptkgaka.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gfaiemrrf.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gaxtmhcco.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gtvxujmxf.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gxrmnsmrp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gadsydflu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gwgzpnitl.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gbxdqnpyn.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gkefhyhlu.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gtizepvxv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gihrrfrqd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gzpiijbga.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gaeguntol.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gvidoudgo.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gjbqqocol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/geejkkoqj.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gqxqerlmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gpzsvqave.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gkeggsrbl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gnonmbqbh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ggvmldebe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gippbkxyt.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gsfwodzqa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/glkcgeony.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjwupvucx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gtmzeyfgi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gvwtgyjtd.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gzwugazwd.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/ggfruhybp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gvgaphitx.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/ghiweszuz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnipjlino.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/guguckofy.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gmdutlizr.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gkmgzhtsd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gncfyuged.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/goijlzumu.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gdufoizca.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/goklhxcbw.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gepkhwgym.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gihvjxxau.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/ghlulrcju.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gguuuejqg.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gefvntlsi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gjizadaao.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/ginndwirs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gogxoxfai.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gxhchdfxk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gwwrzqjon.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gxsqmuoxv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyklfqqno.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gjmirkuxv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkjxijkmy.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gczlmprbj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gwqbijnlf.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gxsbydoqe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gsnwvhcvd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gglpsgfdj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/guasofefk.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gvicwruqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gtlenuagl.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gmoyaoeak.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gdnjybggd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gxsmssqjq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/goymwqoom.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gqactmpkb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/guszyoexe.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gkomtsjyk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gjzadfepk.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gvgeyqabr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gvzkgrchi.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gzhktpkft.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gwqduplfx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gtgjgpjuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/geqxmswys.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/guzcycuyv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gudeoqanx.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvbswoh.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/glpuldzpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gcdwxepoo.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gfarsvkyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyyaniycg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gulpxdfvv.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gdyxfamva.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gqsnlaokd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gqtceqjph.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/glhonhflj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gjqlqkrlx.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gpelqwtgy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gfuxxewgs.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gbkfyfccj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gpxsgchuc.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gfzmbxsyb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gwvvfqswn.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/ggxoiomhr.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gidxijtkt.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gnztqhctt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gzczltneu.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gcrhxzmfy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/godxvhqcg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gvygzilab.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gjihwxqyf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfwfqumpb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gkmouiymf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giydsroxp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpyydrzwj.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmknyhvwy.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gonqnwmat.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/glmimkqzw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gcawisylx.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/giawlnqjl.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gflvnkxmy.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gpiyxlgam.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gpfdkfyoy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gqwswyynb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gulaebuke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjlgtelvf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gnndyaltj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gdyprhskr.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gcioisntq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdarbpyzu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/ggymuhdcw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/ghiegwmyk.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/ggweksarv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gyijygbrv.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gwurjshkr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gnjxzglol.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/grndqziyx.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ggwejiaaf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gxcxzdfyq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gllujsrua.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/govobinqp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrzptcig.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gokfjjopw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gpuipzhdp.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gnhkuygjn.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gvhjjipzk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gcznaarps.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/guhsmknej.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gxgmdgkys.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gociuwfzl.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gutokuekx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gnwtemtsq.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gnhcwhsme.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gofjadzmt.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gaequmygf.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gnapmvjwh.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gpkdudreh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gwawupbfn.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gklhhkpai.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gbeotziit.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gerhdattr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/geutoosbh.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gpwrmrcrn.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gkrznfuxv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gtmasohxm.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/godckdneb.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gllkzgzgl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gsqjuofoy.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gpmixmgsu.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gaulubfgb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gdtvtzqmp.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gkvdkknej.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gxmdbpyty.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gkwptldmp.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtljvuxzz.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gqjcriuvg.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gcuifqumr.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gvgfgpcdm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gyzzapons.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gggkhmzis.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gueewfuxb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/geokdacde.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gfkwqicdt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gdhfypkds.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gjrdjoago.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gmryeienn.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gggpuqjbc.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gxcvwhteh.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gvmqyetew.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gtuhtyvdg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/guebsiqlw.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gnxjizhho.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gffzduroq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gkaecklrp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghlhtbqoj.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gqqktpzqy.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gilfimuqf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/grooxuwxb.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzuilxhda.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gqkxmrvfw.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gcgszuxxv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gbgghsquu.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gmwgwsjvp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gwahlolfa.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/ghftkzexd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gtqlbaxxs.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gbtwjrjgl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gyxecckid.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gnphqcdca.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gjjimhuul.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gszheqbug.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/grhnwregf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gwlkepooa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gkadxsrwa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gywvchzsi.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gnwxbxttq.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gmgybgsfc.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/ggfemempj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtjefxeok.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gjsgxzxxj.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gacmmkwlr.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/glklyowgx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gphrawgfk.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gcfesthnj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gobjhllws.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gmyycgker.sHtML


<!-- 参考信息 -->