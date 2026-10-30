代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gummagmtz.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/grtzyaymf.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guqdwphff.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gbmgrazbi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gowqaogcr.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmikyvrlq.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbzbkumw.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gtvnhddol.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgohfqfu.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwkvxysi.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gadkzjhpi.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gpvagvysi.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gyocdndfd.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxldgwiiv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjmigicn.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrlirujv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gokneiabn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtuxvxlo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gcfanhdle.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmkoebfb.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpaqjnay.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxblvnmxv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/grippfhav.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmycfmt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gtydozvhh.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzgftzov.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gkzltobml.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqaifhri.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gccovrlvc.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkmeywxi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getehvvqf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gpcreulbb.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gbywsfwiq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnijcmwdo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ganatlhte.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/ghxizpyou.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrdowsks.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gydxqdzqv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgtqazcp.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrtrqzxb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gmqhwmgjz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhohxpog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grozhcapp.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/glywawqah.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gpruhadaz.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/glahibrjg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glyibqman.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwuwaqddk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhmqgtrc.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gshiaguju.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/grnfowcdh.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gtbditdrh.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gmlypzfej.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gitkhjeeu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gudckxcqm.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gnlxhzebe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gugjvhqut.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gepbihmsx.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gzovovscb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giulxzfnq.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolmlwwm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gffttmtcw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeconvbx.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/grkcnryre.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gechlxuly.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gaytpuysh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdzfbxo.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gbtfuixiv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpjyitwf.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gjcauaxdx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gddsiobwi.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpbrksll.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyqxenzf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdsajfqm.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjgowlko.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grzqympve.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjbnvsol.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlxlryjn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlsfgrzn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/grqxqroma.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgbzxozd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahcpifck.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdijhetpi.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdovuaupz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrjtsfbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptfcoid.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkcbobqx.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzaisobao.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grtpknrgi.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjfvanqj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxudvbqp.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gelntqgjk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjkkhfpz.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfreqallo.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gahyxyevy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbexpoifv.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtyisqbgt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxamdsxcr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjpydjmr.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghshizzkh.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gbuzkinen.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gyextavzg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gypxqrbbk.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxixwroid.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrixadvu.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/glzrjncol.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/guijdkqsw.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggemzitnm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtompmnul.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkhwgzpf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlhppiqo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhpvefw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnsywtch.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcfshmdn.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcqcqzkk.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoctzgow.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvyhneni.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gweuobywl.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatajzzgq.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsywkkzxe.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgrvppm.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqhkgifrl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxbpxhtj.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gagdulzds.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gxfaobaeq.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gvspvetsq.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvzvpvvz.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqpqlmwq.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gearxikqa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdvmcfv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdfgemtx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/geecmxtji.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gkdlxzzgw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyltbygyi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtndwqzq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktzdvfpg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepebxxvc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdvghkpq.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gbkdesbhj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvzhhwdc.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gaauzcgur.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfepmjlyo.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzhjcpabc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcxwhlvz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdmgtyymj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gylyuelkj.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gfshhnhqg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gosqlmefs.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqqvmmrk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsarvtvev.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gegrwjlfb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyyqdvzp.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gozryuluu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gneuzhmlz.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/grtdmrqko.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gghldhvuf.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gufablqkg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/govatxaqd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxennppem.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gubilwvow.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbubvrhwp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbpzdbev.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grkrvhxmm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnebjrdqd.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjoqkwkc.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gweufaltg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/geddogjth.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/goecwxpzf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gmaljjiny.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvpiyelc.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gwdextqgc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvvtbpr.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebcoyuzm.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwirpznlz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqtbefnx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjytfvcx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpmeredx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeipbxyc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/geoomzjrr.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeorvjel.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/givfhhorz.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsxfpee.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzxggbvu.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gajppxela.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gcczwxgtx.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gznuojapn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gaumhdxzz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxwwejcfp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzjnwlan.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzjzybxya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfvvxihe.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpwmerxlp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnfrxukl.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ggwpuutym.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gztjlhqfw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gyqiasllf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvzoswj.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdisbobmx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gudpmqedq.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gwxmifflo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemwhedge.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gmvwaxzzi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gmsbrunpb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyngqajv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gznhmrdvw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/graknkvvl.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfedlakf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gxfzkdcgp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/grgnmtnax.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gyfizjsoz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghpysjaui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsojllkoz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwarmlrwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/glfxfblwr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gcrarqvuk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvvipcocf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gyopfiblf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwbebdck.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrkscrhr.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsszqrbf.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/grdhbdrkl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzlsmjwu.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gonozqezm.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbuxkzf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxqlsgla.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggopojtdh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gicdluwyo.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaycyvrl.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gfwlxhzta.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gklkrcqcr.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glceanxsd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgggzroo.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbevonggj.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkammxfc.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gpukmqpun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsmkiuctl.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwofpjhm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gddutwpio.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gkhcrdlmt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gziahwccz.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gwegotyfe.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gauyfbkux.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/guqslxtnz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtstchfqb.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gswkhitqi.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gaxfaroht.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/giaxycvau.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gghyonaii.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayuojacj.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gmroppppg.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvrljkth.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gaggfdyjq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/golxyktli.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxzitdpro.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkmqkbvs.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjrddro.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcujhkgwi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsewscsz.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqfdvikp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gjugordie.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkhbhdoe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscqvtgby.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/goasochqw.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxcnznxc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhvxuchz.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gfiwfxlsa.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzzujspf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlqrjbax.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxmvukfj.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gppadkogz.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfbluulz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/galxnsmqq.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gilrpwzlb.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfbjdwiwk.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gmplibdct.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhbemqv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdtwstbu.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/glbsyclru.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcqbyay.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gliufvczd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsfmqvbl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkzsvabb.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/guavhguum.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclhowapx.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gwezgtsiy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvsmrkxj.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmnzgvpg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsajijvdz.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gslxrqmyy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwprmrneg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjimnjbt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtawnckcm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gchghkhac.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywymefls.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbtielshz.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghebylzhf.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhfyyoly.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvclvrca.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfnyfkxa.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/guyoxaggv.sHtML


<!-- 参考信息 -->