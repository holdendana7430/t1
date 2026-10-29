代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gldokqubi.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gsuaviiqz.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gzntuwjrm.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gihtaocqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gbiqbrdbw.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gorfbstzz.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gtbrgfopt.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gelcewlmx.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/grhrewefl.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gbnezgukp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/ghhbqvkuf.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gvnppfmqd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gheditlrv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gmrguhvwp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gasqyolqt.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gijfizvby.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gtwhaatrp.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/goeiukufq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gnengzthy.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gfyuecwkk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gystkonsy.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/ghuzygssg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gctftgxms.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gcbgpzqjj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gjymmetvz.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/ginwyupuk.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gocnnshzm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/glshzwbuo.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/glojhidfy.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gguajnuug.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfuohdzda.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/ggujzwjze.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gktmgzfgs.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gsqlrsbuk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gagkhdnxs.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gqkxzngxu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gbisykwyu.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/grlrpvqdd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxrfhkvba.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gxgqwcqdb.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gciicspne.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gkvbchfey.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gyfqmivah.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gsfgexidp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gmlkaiyxg.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gshnknash.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ghothvkah.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/ggwymdsiv.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/grdtauawu.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gcggqrdze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gxtopbmqe.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gmheojnit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gjvndjhxk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/grhsypixu.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/geppravxk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gajsxtoty.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gqqxyzlax.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggcwvzntu.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/ghjmzupqh.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gtyiwuhtn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gelrzwvly.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gtvktwhof.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gixnpqtsn.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/guozuaale.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gmuffqkla.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gqwgfvznu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gfctmqvyx.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfztfdpau.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gkhfjzhqn.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gufmnyiys.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/ghzwowsvs.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gkdxkkocf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gmqhpjhlh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gjqgjispb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gquiinmsc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gmzblwvtb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gvovcqsdt.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gxwpvqbpi.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gnqnzysnm.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/grhtjnanc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gvyqqaclw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gbzezvyvt.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gusxrooto.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gigmbytsw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gmlourtcd.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gmxeqmdtr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gecskbgjg.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gbizogwxr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gjftkshcm.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gmnturjii.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gernnhtrx.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/glhasytfh.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gncnmbmpy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gsgaryccs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gfkhwzrfg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghjgremdp.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gswmfdnqy.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gvopjoqgt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gyuiohpsi.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gvcjqncbd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gzfyqfgff.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gsserzozj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gjpuumsrd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gzwrrzyfq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/ggeiybqex.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gpwryrtbd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gkhmiyllq.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gkjlskdgq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/grmwplmuq.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gxwqrttfu.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gwvbzmgsl.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gkcxqooxe.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gorovfeka.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gpfyzplly.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkotfnufx.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/guqxfpjvr.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gdlttgmgj.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gwftvxrdc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gsiyjnkmp.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gsydmodda.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/giosbclbi.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gdvywjsao.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/ggxiydpat.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gyhxgftjj.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gkhhsgddi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmtikzalb.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/grjpamhsi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gkzcwrdvl.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gdheuhcjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gectyfhjw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gogdobyqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxhzstns.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gadicpdvi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxkjkplme.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gpnasijuh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gubvezjnu.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gospyuozk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gfqvhjqfv.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gqwkpqekl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gpfimprxz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gvlmtbwbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gcvoghwrl.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gdabvxuwy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gdmehetkd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqldlasvr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gmcjyuqge.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gposdovzg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gxkkzdagh.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gltqhlfgk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gvdjudknr.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gtxgjzqiy.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gflvarasr.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gbyakrckk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gkfaezyco.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/glcmjtakw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gjjtgditi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gubywrate.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gzepjmuhd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grrapwqla.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gpkbowcue.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gbtgudmgy.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gshnmubqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gartllcyd.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gtcqpiooo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/ghkyxpyfe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gxwgmylle.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gdgkwschh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/ggcdqgpqb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gagdksnih.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gphcovngr.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gznttgtzu.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/guwqsqnjj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gsvtasuro.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwxawhd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gvcaggadw.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gpfhsenwm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gtjtaazae.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gkginhlwr.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gautdggnv.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gmqijesgm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gfjgwhlub.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gpoucynoy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gjjoxbpmp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glhstvdoo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/grsslbidv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtmtqllii.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/grwfcfvnh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxihkdrgo.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjrwzgwml.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gdhbrifhc.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gtdjpomwx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gkzttztvf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gaczwkrsf.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/grgrphvik.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gqukzavyv.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gyafqgwea.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghdmwiodr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gkkxlsqmo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gvhdbmmpq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwsoamsvy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gksezibix.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gountvksv.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/glvlpiqky.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gwynihbac.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gmpokysld.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/glosaplfn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gcdozeljc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gobyuzftz.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gqtorhjss.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gdejkvwdq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gkpruvbnf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gvgycuyzb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gqcqmpqqn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/guehcigox.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gqyflowxi.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gcxchbgvz.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gxkohmavf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gumaproyb.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gekyshoqi.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/germhnsnt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gbyckmiga.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gmkxgqspb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbkzvbfki.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/guqfbqqxl.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gvlhnbped.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/grjvwneit.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gbfwyzfjv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/ghnxnlfvr.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gjyntohsu.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gjlxmutre.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gxepvajqr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gptszyfas.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/ghitqtrjc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/greybgdwj.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gobtskcul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gyjhawuaq.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gmvmyjdwz.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/giyrznacd.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gatviienu.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/ghrtfyoiw.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gtgwuxovu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gciuyaoqa.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gyhtdyguo.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gketxqbjn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/grmxbmimf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gudfesxkt.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ghskasxcv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gwclcsyok.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghzupwarw.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gdajvhnhq.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gpxcvinxv.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghowobezl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/givnjyfki.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gkkvzrkpe.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gipkezitx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gjkzoyiog.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gjrejczkv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gbeqnalwy.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/giiwnqabo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gyxsbgpio.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/guulbuzhc.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/ghqrltwnd.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gsbkvndne.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gfxbuqnlo.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/guiirztzz.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gbrnygpsq.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gypuyreyl.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gjrnqkarw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grvbrziwe.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/grvajpamu.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gvtxxjxvv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gpuycimjm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ghqnacnag.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gakvyspzg.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuogjwe.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gqxtexdjj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gudkrsczp.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gdkxubfag.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gwlslhlkd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gdygphcle.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gdybsvgak.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/ghuzdlfql.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/ggyteahog.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/goihmmprv.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghkqgoexa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdhyoveeg.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwkztpoyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gvibgxfnw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/guwfakgzl.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvsnvdjpr.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gzkhngdoq.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gdoqtqrhi.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gbnghuyhb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gixpiglis.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gghpnytbx.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gublaxyyg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gxvfvgzfa.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gqvjjdjhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/glzezxens.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gcodsrthl.sHtML


<!-- 参考信息 -->