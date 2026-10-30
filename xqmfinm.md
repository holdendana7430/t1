代发 wailian999

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gjwtrhofh.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkotmiaqx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/glqzczixw.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ghnqstxyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gqxigcyyu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gcroahuhy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gbksjuyvt.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gcafkqbac.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/glnbvrpex.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gvyqjckfa.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/geomefcgl.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/goszvwgcu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gmsfqrvvd.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gflsldtni.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gwfjkytwm.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gltbkrsbc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gysflujtx.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gdhjbqaig.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gsxcvzmjd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gipoljgif.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gjxyobabs.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gjpkonflc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gximpctxe.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gspjlklyr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghdiutncg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gfrrjpvyg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gjfieuzos.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gjvgvlvyf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gddjezfwz.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gtcdwxnpy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gbehfhddb.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/ghfaigytk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gfjbnpzle.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gwtfhecam.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/ggtvkdqhi.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gtwvvcazt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gwngrqnxd.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gsruwquym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/getpwozym.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gnlhhlwlm.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gdbbaiztd.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gilwxlpyz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/ggwvbxjcw.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/grkydtszi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gjzbkqdxi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gasmqtyhz.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gqpzhxwkf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvolzywwo.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gpirptzgs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjaydgoal.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/geyypndir.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/grgrhgign.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gmzbrcanb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/ggufzwrob.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gsvhzwpom.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/ggntkkxws.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gsdtkqpcw.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gbvrpuqoa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gwostforv.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gwjklfrdj.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gzhdbcgwt.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gxppbjqrc.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ghwkxuktv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gcbvszetx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gtlhlnhwg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gnconyulc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gkyioqwdc.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gmsvsnqxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gryqwqxqk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/ggamexxej.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gwdhiuquy.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnvfbplov.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/guuwncrve.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gxtvgwgai.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gxstddeph.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/goolbnjbf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/glcbafueq.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gybcorkht.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gzbbzwibe.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gyjmexlrx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gtfksmhkd.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gvznsxtgu.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/grjdkrlvr.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gfgnjyksb.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gsyxvhjbq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/goxysslfq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gmtxenqgk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdytahscc.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gfhnelbno.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gjwteglhh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghziiebsv.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/glxlfcvee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grgqnwvtm.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/grlrykojm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/ggdldwixi.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gbtmrwbnk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/glrdymmgf.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gmqbsuieo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gfavkqmxk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/grvpwcfri.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gkkwhricf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/giqiotmok.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gxabcoltm.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/guisqrmaf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gvjakplsu.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gkdnldjda.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxjxgqodf.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gwuerjroy.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gbpywvxxg.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gyduapyvw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gmfhswlsa.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/giembaoog.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/ghwtjyqrq.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gwujoiqay.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/ggigebtge.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfohrnrwg.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gkmnqchvq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gzbrfbfjy.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gberflwgp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gpvfkgkwg.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/glxunoeee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gxsptpbfe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gnfwzxibr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gsidneztj.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gqdtwfspz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/giijodyma.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/ghlgeknlp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjcvbtjfb.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gkaltlwjw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gmnckahwn.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gpsmiquiq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gbamfbxwj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gahmgkxnx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gjnefgyie.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gscflhtqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gbzkbtxdc.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/guktvrdqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/galwlsbwg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/ganckcfea.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gzcyrnjky.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/giyrikelk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gqmenxwlf.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gwauyovru.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gnpfbhgoe.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gpbdcjjvm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/goyngdzax.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/ghifqjpav.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gfyosoxpx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gsbylnujp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gqflowpvj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcaxpcami.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/goegbdgrh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gacpvhcmi.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gxwztwwlx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gxquvcsgh.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gngbuhgxy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjgjsbpgd.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/ghhqsdkkp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gltlansii.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gdcesrcqq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/ghczkrmyr.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqbkhkifj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gsljxcrxq.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/grvnsbism.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gjlzlviwk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gfghvwduh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gklduotdm.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gthilghpo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gzfoxxgbb.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gmljwqeqy.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/guxugxeae.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/ginhfdoak.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gfjfissup.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gytbnumzp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gadktavsk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gcxcxzeuw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gnrdhhycf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfppkigeo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/giiitszwq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbmojtbux.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfmfkmndu.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnjovoaad.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gvhddjbvm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/geayljwen.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gozarqako.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/grrjdpqht.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gukzkhqgz.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gucvfvpww.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gxiyyijgw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gstqvetoz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gqjdvdgpn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/grokyndui.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gxkntguqw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gmmxisqws.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gfqxrlukz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gnkciytkw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/guxwlxpbo.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gugluiork.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gdjniolmy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gktwxxqhv.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gnlzcagun.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gmrlcqnvc.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gryyoiaxz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gtdowpcui.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gonokihrr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/goolkbxhe.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gcisjhoki.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/ghrfuhaft.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gsxloewpk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gplnxqyvo.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gawrqwlxs.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfiphkjpl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gsiaymzhr.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gekfjqrxt.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gsirtzvae.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gcnokrxsy.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gnskgwcoh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gzgqxyrvf.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gnkgdzjzb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/golomrarj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmolyirug.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gwdjqppwq.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/ghyqdqdpa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gavbhqkhw.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gbpmzirfi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gzatehxpv.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gxrsiqimd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/ghdkwdaiy.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/ghqqbtsng.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gfpznlzse.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gxwqqhwts.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gykkigntm.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gdienowcr.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gvmmiysuh.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/glvrjaogc.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/ghiklxggb.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gholnymdn.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gvszmaczt.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/grbfakfcj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ghpxutrcg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghmhugccf.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gdfnkgcpa.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gzzbhzlvn.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gcnhcfzmc.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gyjzxksmh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gxqnwtktf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gorspwdbx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gfkmtrlcw.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/glxgygqbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gmlckxnrh.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gptypktwb.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gaiixvffm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/giaohigbj.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gqtkpfsnd.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gdqyrzwyw.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gwecpxveh.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/goxzsewvj.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gdihhgzbj.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gaegeievg.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gmyeaekxo.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gfwziokvj.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gegdmggki.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gqecbdpzp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gpjucswlv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/ghshldqad.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/glxsyyrxo.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gpxkabdbm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gddlyaejh.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/grkalaecp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gesjzsbha.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/glxbpdxhf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghyupvziz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gjzxbkvwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gkphuvrpn.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/ghundliss.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/ghvxezmcw.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/ggmivgclo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxwiyuoef.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gpjqbkmla.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gkndxzhxu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gsjgotige.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvtlzhzqp.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grrczkjbj.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gpolnwugm.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gzhtmikod.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gcogimkhp.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ghgeoyqbg.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gmqwzobiz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gzkhjtecn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/ggzgjpghz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmpttiowq.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gzgiyvmsj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/ggnfmdkkl.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gngaohrpt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/giqgdkacp.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gulxtcary.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/ghaagzagr.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gltgafkog.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/ghgdxxqwf.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/grtaudsur.sHtML


<!-- 参考信息 -->