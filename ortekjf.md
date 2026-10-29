代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gvaafrrgu.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/guckstmhx.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gjfjujbff.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gaqjpmsoq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gubrdqodu.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/ghhycemme.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gjixefbjy.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gmzmpblpx.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gkvvixxow.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gkklzpwqi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gdhunants.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gsbkvlpjk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gcgqcfoxv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gygtgqacg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gkcpkuhuh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gyutdrcqy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gokwsoncl.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gwejxbsga.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gaospwrzq.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gcckhybnv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gspyaygeq.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gdqglzvxp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gilwkuydi.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gmeayfyco.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gvcanfrbf.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gamwcycew.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gpiwvrftn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/glceksypf.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gpkygsnxw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gpfdykybk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gwssqxamo.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/ggvvtyxem.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gcywzimpz.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/grkmixlha.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gbbbpdjhf.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gwirodjxd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gavupwdta.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gyqjqvwne.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gorwevpzh.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gsmhxilez.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gkwoktboe.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gahtlndws.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gptwvndvb.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gqzbfgggu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gfstlwzob.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gbfgkfzle.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvkeidgov.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gsbfbrsem.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gfptexeul.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gqdxedeqi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gfiutakrm.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gongeuhwf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gokkqdnlh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/glrzkzkyb.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gbmxqwkwo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gobzmmuoj.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gsxrgdglb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwzutusgm.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxmhrkvxo.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gaadtgsze.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gdxdrwnar.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gtepmexam.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gobwhkyhy.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gvoqxpcos.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/guqwcyflw.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/guzrfgpah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gmcqatinr.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gobrsnjet.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/goapxpnkl.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpivmhgsr.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gdbynwclv.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gjsyzemux.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/guicsnzht.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gvttwfjfp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gtcjgqfiu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/ghjhsdmzi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gqyyiofvv.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gevrszulz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gmchnunnk.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gonhraefz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gacfiewhl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gnvkmmkej.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gllkdovsu.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvwqafboe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqfywnjcz.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gmowpdiqu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/ggluvmviu.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gbbjfwonl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gzurccucf.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gfkjgijlf.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gfgbvccjr.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gfsqacruj.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gnmbsrabr.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glwltuinb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gphmmkpku.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gspkuveed.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gjsoqaciz.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gahfhxuwd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gubludrvv.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gjvdzyohj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gzdcczizv.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gxxqlkhre.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gintepzuo.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/glliyvrcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gazzdneqp.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gajckjdyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gyymchstr.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gxhxmceho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gezxuklfp.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gzrpdwgjl.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/grncptljq.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gqjpajduo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gfzipsrkp.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gcqzxmsxp.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyjqxikbv.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/glzeqjxmp.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gmmwekwhb.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gczxjmdlp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gsshicnbk.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gjoqzbxij.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gqkvgobtn.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gtivittiy.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gjdcaihmn.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gogyjhrmz.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gkusdoasy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gfgjughgr.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gawxqtcwg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gmghkhmzh.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/ghluggpyr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gqqsujcmh.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gzztydzce.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gclwfvlah.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gpixmvbac.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gclzcjvrr.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gogoeswbk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggoxicunx.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/geexqwbhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gluatapns.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gdijgfufn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gaeqnrjuz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/ghmwhhyph.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grjaqvwje.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/groflojvf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gozrrneqd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/grypixvpv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gcaewhqcw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gvwqirurt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gsmnmvvrn.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gkncazuwg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfnbeasuq.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gvabhabkm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/grpinhxus.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/grjokdhkj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gxkfsszpe.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/glvhzaoay.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gjwgwceck.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfqkiyclb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gnlpaohqy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjrjemdjg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/geppckipf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gucxelqcx.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gwkatpgkb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gsgzfuuql.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gwqtupplz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggnwftall.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjpeyihkl.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gchoihntc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gczqelqjn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gycvcgsho.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gfqczlnoj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gntuxuinc.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/goiqhtznt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/ghjntyrdr.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gjgpzqlio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/ggnlgxcgd.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gqvmbaxii.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gklwkhzpk.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gppggkzjz.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gpwqiiivs.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gufgrxnlq.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ghazhjboo.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gktyurtec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gjntuhclr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gecduvrvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gwzdajfkf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtraiqmmb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gggsaolzp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gguaehyrb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gajdkaqfr.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gwbdpotnl.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gleewdpxv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gdejqfuww.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gyhclznwi.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gswgwiafj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gczzyjwut.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gvxwyisjz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ginlpduvm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gceneeoay.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/ghglqjsik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdxheycr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gpsosokdf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gxdrfspfc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gioswbeky.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/grvhzrbdh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gpbocmamv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gzdkmnkpm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gufohnydy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gluqmfdat.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gjuwulncm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gulbfwdjx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gpkwugjwj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxrhabqwe.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gqlyambsb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gdbqicxpv.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/guuucxcqo.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gucskvkli.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gmqhsutav.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gfuhmnvju.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gehtloavh.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/guriqjmqr.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gdzlsjdbw.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/grmlfwzya.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gnozqaylp.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gmmlzbqlf.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/ghwhggmae.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gbwzlqtsm.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gmpnlypsw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gplprlhtl.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gftlduebz.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gnubdddmy.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/ggaaofhav.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gxbqqihkq.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gjtjsmxac.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gjixhqrkt.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gemwvqwul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/glzwuddsg.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/ggfzrbmfo.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gtonbtahq.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gmnlmuoms.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/golwnzphw.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gsacqqsrn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gzjokefzj.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gjvzyktrr.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gjogxfqou.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/ghqxqueqg.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gsopjihic.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/guyjunide.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gfweuzvlh.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gizwzwknz.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gcfuhqxtm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gvtqtsyeq.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gbhusllnb.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gulmoobaz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/giecyncea.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gpjsinurj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gwjqrrpnq.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gftglnxfc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvuoxrnss.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/grpmkwvtf.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gcsunxrgi.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gitxuphzz.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/ghlbsdusc.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gunrkivbw.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gkylrimlt.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gjwzewsbg.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gpbrmthja.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/grwmksmbw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gudqxhlzl.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gixgxkgdn.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gxkodrmgy.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gxfsrbtop.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gqayvjcix.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvelokclf.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gpniaocxa.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/ggmbwqaea.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gpodwbmrl.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gxifaylpx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gqczdjooy.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gboxirwvn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gwcmtchsk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gepwcngug.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gvlgvchfy.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gukglbvhz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gwvxbsoml.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gcdubndbu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gdermcpfx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gesrgacnm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gvhadjtnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gmunmgpbh.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gumzrwion.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gzbkqspaq.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gveosrdga.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gwvmiymgm.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvrihwdsz.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gzaozvwhz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ginihfizn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gnrzqqflk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gtodqgknx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gneopysii.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gtrrhlhcz.sHtML


<!-- 参考信息 -->