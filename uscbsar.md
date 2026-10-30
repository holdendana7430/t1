代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gmkhkibce.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdvqpddc.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgckvoka.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbmpmobk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghethsgkx.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/glekmbwmr.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gndpjvtva.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gdnxrecow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrqsdixz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxsqbcjl.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwmnaddd.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gxofbnxkw.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbfixwti.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqnavite.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gtjvojdyn.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwypbxfrl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxqwbko.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijgydukc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmtlnost.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjvccrs.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gpgchwhgp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcnhoahbc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gkllsqbmx.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gxmatniyo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtgdkpi.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gursigpbz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gqbwillxq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrqkjei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gqqmdrelj.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/grksdtfsg.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcidjzhub.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gvdggyntd.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gkevuafvp.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gejqkswmg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmosbwomn.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gavriwofn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gihdriynh.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/grkmuzfog.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gmmbcuimb.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gbmnhcdqr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcrubucy.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsqogbkn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxjijhkq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuabudil.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gyyicoelw.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gqmlimnxz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpqdlefbv.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnkgftuh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlumctii.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwhfiokp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gyivkkxpk.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/grhsskixr.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxgvrdmqp.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhdvuhiw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdklwfkeq.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzuyknxy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjjurmkqq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnboxvkew.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/ghovjsxhs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkvtjyspc.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbbxguzk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpcxethe.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gstfyfyac.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gtpnwugzg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgbxbqlg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiqsjize.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggywodbrs.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmrmzdoj.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/ggztmtkjq.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gubljkxsr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgrzvxhm.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbifzpmls.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynxyurtd.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdzyohdaw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyziyixmc.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/grnwmpezj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdspdxazy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gfvqwsmvg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gtckdpsoe.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgiwlrd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/grripndqd.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjftfeigi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/glgffocts.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnqqtcsid.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gpuupdxlf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/geuufdpvz.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgegdegj.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxamycvu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/giajfwnxs.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqpxbfp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgozney.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gztrpxniu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gktatdudo.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpqinbxkf.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdaoqxieq.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyyfypis.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gwqpbmvtf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspdemolw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjhpoyba.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjtnyinos.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzkqmsfl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdkgshxuh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpevbkqdd.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftwvnvg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gygxstnmo.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqgybznv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gdnhmnkmi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxbpcrl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/goarkfpub.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwcadfhe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscexojqj.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/goapczvpw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmqnfmtg.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzhvugme.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gmaknszct.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gqheupnmt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxvfmyszy.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/guvurjyhd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gderptkkj.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzhtznks.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gkrljxtap.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjhruqbcj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gsxuxplju.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcczibym.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gjpfcerec.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/grzklatix.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcjmfwva.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gstxxqbgh.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcijwadk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpyeempc.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqagyapo.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gjhganeda.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gentsgabk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxvxhlpq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqwlvmdl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkxysmzyx.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gjfhnusoy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyulkrjz.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gatskxqct.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgslianc.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjpintwg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhsrwols.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgqhyrmz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gyubnlrob.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwoijrysx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrykivmj.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrguhaiv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxcabafes.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjefitbqc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdpsqtci.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvptgcpdd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbiqaom.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloflhvxs.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gljyqbdmr.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrksmkp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghslowtkm.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gdchxhqgm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/glcbnupjq.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gdqadervt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdycfvyh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giujiwqjn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynrdoutl.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gruhfwglc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjieezys.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggelgcdyu.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvajmyvd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gopcznexh.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/grsynrynx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gykyeyyfp.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxiwzahdh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gxsabncyu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/griaqfejj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghkesmdoq.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmftwljbs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwmjnkio.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gyuuusfqv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtftcsf.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gwefqtphu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gnuouxccr.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gqfahxwya.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/greabvyss.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekkjwvbo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gualxucpo.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdhodsuzq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzyxhcoh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/glgrnvrmu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgkzordf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzhraogy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/guiwvxpbx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gshezacya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gutmlfawg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmmofwgpj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnucvmkt.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gezwhaofl.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gexppngza.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gtclgzzbg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwclvsds.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmapivwfu.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwkjqln.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gallzytwp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvclziqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbewpudd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzokjdiec.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnwjaoir.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnuzfzwdl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjgvgdfy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/goulhwjrj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gbpwpawkr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gladiutji.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgwevyzf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gblchniyp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gvoatsuca.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/glywfbpyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/grnpgpadg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauzsdeqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/giakhrnui.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnosoapj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gleyitjod.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gpnwrctjc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkuuqeds.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxpqpzg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/grtbafxbi.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grjifojoh.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdluzrbia.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeypupsa.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdtdxmxp.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gokwgihox.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gowtinwgg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibygnsx.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/grrkhyxjy.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/geinnmyrw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/grflosmga.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhznijzr.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gasegyudb.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgugogqc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmvueqotq.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzykumszi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajdydhhu.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gijpawmtf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/grskcsfib.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/giexdprir.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpzqztqu.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gxpfdkmee.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gcexrixim.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrnjbgnx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghglhmydx.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gumrqapuc.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipvkydj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/guobbsfcg.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gewyhksvz.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/grsodvewe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgosiags.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdupushk.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gazzhabmw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeyivhed.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grawbtbem.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giobnusqn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejebmva.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/ghzuuwlta.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gbljgogzx.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gedmlfajv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gedlvkjpw.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gduhwjjvw.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnonooqb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmiggmgv.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/grwyjsnar.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjdqlantk.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbywsdks.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdxucdct.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gkbrxkdut.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/goforasjc.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gbvmfucgg.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrsdbkfb.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gadldiuau.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfobuvajh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gtnekcfxa.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefzgfjgh.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyscqove.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glknglrxk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnuladfy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpqngusr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwrrnxwx.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/giolfdnim.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gysxutidz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgqngqbk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfiimwbs.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gckzokasu.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gczfuxfvy.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtuicsjxh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gktddrfre.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsiizwci.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvmekcma.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvtzivum.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/groaoxjyc.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrktsjug.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwozugtnz.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghwzcwtqf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpzfqtk.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gplxjpwxk.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscywlutg.sHtML


<!-- 参考信息 -->