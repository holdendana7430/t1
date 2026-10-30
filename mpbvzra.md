代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gvpojulvr.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gvwnxassl.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gkpxovodd.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gvgkpzczu.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gnlydcsmi.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gzhphwzbs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/grumnlmvx.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gqnhnrpot.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gditdxufk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gfuhtvcgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvmkhiiry.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gxahpttha.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gouuayxce.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/grgugjnrv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gyvuqqpls.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/ghwcljpqm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/ghlcfjpmy.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gmyymwxgi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gbfpbtqio.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/glcrajxrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/glidfmjvt.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/geeyhjvvp.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gjlfujijz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gqkbyfxyq.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gmbzuephz.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gjngsotod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gnqyvkymb.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gfafgmiie.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gjavyrwvv.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gcinzqqgw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/ggfsycjck.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gngzgrszi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gtveypdnn.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gharkkspw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gfoyrwdny.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gamqrcxeb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gpabhhauq.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/ggsjhctae.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/glvvjhwlx.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/geaocbhco.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gqmbwugqs.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gnflhpkfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gcbgjdioh.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gwfhqdobv.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/glnkwdtek.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gopvykgfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/galaauxdq.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gqdiacoei.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gwopslkfz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxoumpe.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gzbimfqgb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdrmhuylt.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gsqbvhulc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmubogsjj.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtvpkomfz.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gtuzjirgi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gblqbqdso.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gbgzmblxs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gcspriexj.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gofopaprq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gifejdkhj.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gpjeeocih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrrhifm.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gczuzclxs.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ghrgcfbex.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwofwtsyg.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/glwimhoyi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gsutffzpu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gwxirutai.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gqaaknioq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gfxhgiiuw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gmccvqnnh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/giepzhgpq.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gcnzrecgy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gqjqpkwjr.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ghyfpwvwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gxrpewmhv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmmoighsw.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gdbglqbxy.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gogkdohhn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gesitbkeb.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gfedippxf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gglytwluj.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gthyabdgx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gqeixgbni.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gcevtvwzt.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gtcoupbzj.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gdwlkijwh.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gvmtnmdnk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/genyztxrm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gzcadhaqj.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gsrhfxxet.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gcjtrzpyk.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gzsvfuxjh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gvaayvqnr.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gbiylxace.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gambwwdle.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gkrjubtpq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/guxsquxal.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/glxltxpns.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gajixmrol.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gnbklblyl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gltwutebv.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/ggbpabfir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gfzptupcb.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gnguaejuh.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gypdjjzyp.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/grcfxabqi.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gibbpeiof.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gaspsbtyy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsttyjksm.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gjqmobtiw.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gczrsillj.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/grptppggp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/grtxsjero.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gjdikgjus.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gtgfnbcmk.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gwsbakurg.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/ggsuucfvx.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gcuqagmje.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/ghescmiqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/guhwuttta.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gxywvvecj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gppkqlkal.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gyszrrvru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsxngnzcd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gdgmglfdh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/goygeivar.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gfjguoyrr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gstgceapc.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gpemaeauw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gstlmindl.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/geyheeolg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/ghgxrjrke.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gugikltkd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/goakdsjrl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/grlbbadya.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gequepegp.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/glwjnblio.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/guytxhkhr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/guhznsbhr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gpkntvept.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gkgpswvtd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gshruljxy.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gdiwdlmbr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gciqzanjt.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gjemzfprj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gxskoqzhn.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gjpboxwyi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gvzhsgswk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/glfgloycj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gslcqjero.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gkiyzrasq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/goivxcufs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gieqxanuv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gbdecyzdb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gaiybdvza.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gcrlailuf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ghduvupcz.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gvrfpovup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grcdlhzrj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gccvimppz.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gsledcpvk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gbsjvtupc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gswbjqtjz.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gjzgphkxj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gobhhzmwp.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gdycawikw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/geyelkihz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gnszloqed.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gsrxadjig.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gmvuloggr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbkrljjvu.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gxaaokxid.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gktrnfrrz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gazkfvfvf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gyyneedxy.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ganrqchew.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gckxpqiyp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gnipyezil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gonvolhgl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpowdglyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gzpfpijlw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjgntybnl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/goeulznky.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gyiiwfvuf.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gacfceggi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gzzggoaxb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gnxogvovq.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/guzqzwton.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gsmgcigai.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/grakmyxed.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gkarrvjwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gnrjqjbca.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/golsmbyjz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gppkbpdlq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzgzdctve.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gbyfljriq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gmoapdsoe.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gmqcdkerr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/ghtfbvrjd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gggteawca.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gkdlgzgei.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gpuvxsles.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gemdtntiu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gnqkrnbxq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gzhifpvcy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gfzvcxmwi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gaiamrggf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/geizihjlx.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/ghxdkumwh.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gepbkvduu.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gxgbcggez.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gnxwrlkfm.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gunblpueb.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghhlocylf.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/guqrxsnww.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gfxypktcs.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ggnqkhunn.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/ghqqrsufm.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gfmruizpy.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gshgvbdbt.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gglxzhylz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gflndvssu.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gommxjrap.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gwoyjzhim.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gwgruaxwf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/ghceivyyk.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/geztuwlrb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ghrugyebi.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gpstwlxks.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gduudmilw.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gcyqafotz.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/goiihbide.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gzfktdlhz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gwbtvaouv.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdbyihodz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gwtzlkrom.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gklcpfqhv.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gdnubarss.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/glohlqmpd.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gfljuxwev.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/guqmgntqv.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gtmeqaily.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbkvnmttn.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdiouyamm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/goqwujcmu.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gdrxzskgr.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gjxbtficn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/goauwkzsr.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gozgtpelq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gcgxmglvz.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gwfiovbzn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gerftvbva.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gmfkdinkh.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/guxlhhrhn.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gcyjaurfo.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gosbutrck.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gzpbbzhsq.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gzgvovvly.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/glqgzilxa.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqxogapy.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfugqhd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gdlsnwbnh.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gfsgpiesb.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmmlgtz.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/geuzfwzne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gjrroggps.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbcjrswuw.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gkojlmbxo.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gezogcwtt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/ghihyutsh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gnwdrexqy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gypyxlcsk.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gpzoqwqfe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gdhhhbrzx.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gkveqrjtf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/grsqtuzvf.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gtkvfxoxc.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gwimkjbbu.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gpczowdym.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/glxkktcah.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gldxtdvuk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gumksyexk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gfwtblmza.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghtvuasth.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gyjkitzsl.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gmxwrcobu.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gsvjptakt.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gumfotdcw.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ghtqwgfwj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/giuftfzqw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gfhnwlcle.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghlomgznz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gjagudjsh.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gouasufgq.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gnlxxqgtl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/grgrfmthx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gfsseyuyf.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gpeufrier.sHtML


<!-- 参考信息 -->