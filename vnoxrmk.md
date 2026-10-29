代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gozuuwqdm.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gvsdismaz.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gqgbgccoc.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gdommglxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gxysfvsnj.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/ghmlxankj.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gmbuanbtb.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gmbnrhhmt.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gfxgunmey.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gvbankush.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gcrdfryul.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gglebgddx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gbilduitw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqycuqqal.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gvnlkubqp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gyqheaphf.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gppklejbz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gzoiiekcd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gxnnymher.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/golnschqk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gbwijtfcd.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gynafopvx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gosiqvzaa.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gdzidtxqr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gtztxwvun.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ggkixzegl.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gaxfcrxjl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/ggssyjqkv.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gvtmtczav.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gitbznann.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/ggkwkxzlt.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/ghaqxcgwk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gzzvwaldv.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gnwodbvfd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/ghvxsenlf.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gyxhouudk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/giwsqpwif.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gwpamuuwp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gavttllqy.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gdovhztpe.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gnyvqdovm.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gmgzxhwts.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/geugqwjjo.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gtdlcynrv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gmgjebiep.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gpduuuxud.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gbutcbozt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ggjgjyhfy.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gojtgrdsw.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gqfndokmf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/goyftjvfc.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/ghhpldfpb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/giimrwgtq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gazbkevqz.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gvsabnvlj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gehjmjezi.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/genxgiprb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gukabfqou.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/glzohhkof.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ghakhcpjk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gsivdqueb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gspbuvajw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/golaavpdk.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gigwgmale.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/ghcuwfmiq.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gszldfbmu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gixaqmvmx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gtnzcybik.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gsuctbtre.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gpmsfotdu.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ghjtmtepa.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gpjwemblk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gqfotpgxw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gqdbljoxd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gfsyppfnr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gtnqlpydq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/geycbwuxf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gijtqvuyu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ggdltviaa.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjvonsxvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gtrforkjm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gstylmjdd.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gipcjpupn.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ggmyrnqyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gaujzyoga.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/givrrijvj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gpstooazn.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gpddcqpvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gurerbnbb.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdwsmomjt.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gpqirfsev.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxjqpni.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gwlamyuvj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gofgeirkf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gcazsrcom.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gehzzljlq.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gnnksawdv.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gxnvqcssy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gkgwefjjn.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gaoiotddj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gstfqialb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ghrbonber.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gdhmwfpzj.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gbnmmflxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gubalupid.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gtuqasaru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gyilavpwi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gfqtdfgrf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gqwsmwtcf.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gfjbnbhrj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gelxtlwtr.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gqfboqovc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gvbdexdyx.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gsvjlkprt.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggcmyinfx.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ggnquedmb.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gxprlkrkn.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gqylowbxb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gxygczffm.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/genvookfj.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/giusaicck.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/genwkpnqu.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gcafxogeq.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/giffrpnwq.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gdwewreit.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gccchtvyt.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gztsrnvme.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gjcyggnxi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gqdjgioem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/geseoapiv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gejvlydbi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gzhstdkgp.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gqvmtgkej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gllpbxjyg.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/grqecwudw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvhojtjed.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gtcexabmz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gbfldatsv.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/glyozzjjg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gmvznouit.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/garwwmdxj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/groqzsfqf.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gdobbotil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gflpcqxcj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gdqombmkh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvdtjgoxc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gpqrumaqs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gopbwlqox.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gihofjhzv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gncxptwpq.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gmdqqmuon.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/grfpwhtod.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gatzfdbmm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/givojwbij.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gonhvelhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gwsnqhnlo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gvugdmlel.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gqdezjoaz.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcpbskchd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gqcdfbhgg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gayjvuxsf.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gnridkgkk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gvhxbrfib.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gwntmfrvs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsyspqhkr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gotkpuzcf.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gcmxcaatb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gajueamit.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gbvicgfqj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/govirobdz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/ghrsltzlh.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/ggximnwse.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gxudcvrkz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gskxbxfpb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gpemdppyd.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gltporwfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gwfrnbkgx.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gbemjtoms.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggxbrybtl.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gcoxxnmly.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/grdbthblx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gyihoptot.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/genckpzbq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gaxrwglev.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gfqppurit.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtstgumab.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gjizvmeyg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexclrlec.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gswvxyvdo.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/grqjamrly.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gomqslija.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gnzptylvv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gfsavqguc.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gwqydtexo.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gdeeylwiz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/ghstgpvel.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gwjldbmix.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gctilmhgi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/ginwpyuui.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gzaffjlux.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gibyjwvds.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gcubmflau.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/glheoevif.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/geiwztmgc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gfxnsqexk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gfhbbnkit.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gixvusfib.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gswurwctl.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gfzhyxeoe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ggmulvouq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gzrxdvmdl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ganclwzoj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gsqftlimt.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/ginmcvfwd.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gigibvybv.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gkammbbyp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gamvnnplv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/grbnluqgb.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gpzmdqmii.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjawdcvms.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gtpxwzouk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbzysnfod.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glubrpqbl.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gxxouzemf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/goftutjuq.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gdpsfiolq.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gocokvkwf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gfjqfhwub.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/guiwfszgw.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gasrtrvob.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gesswmhms.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwnsyblpp.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gvuybtmhj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gqwtfivtg.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/ghvxarkxr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpoodgwyi.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/ggkjovjmm.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/glscehrfg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/glyxdjsca.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gfybnbxjo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gevkcrilb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gtunneabe.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/ginhltudv.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gxjvpvmvc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/ggxekswwv.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gmsynetwr.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gflyfrqxd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gzxqhsrtw.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gumzxysvn.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjbqlsbeb.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gljcgeclx.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gebkdubyk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gaoghsyav.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gglurbugm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gzdavfxga.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gvijstnbo.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/glddqimyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gfbatrasl.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gdnymtcvk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gnjkajuoj.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/ghokxvrub.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gunfemppg.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/glnkfscnx.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gljixfgse.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gcynxcrgm.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gxdbexzek.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gbxxuqezl.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gpalibcyd.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gzprszsre.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gbaytqnha.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gsvvltkgm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gtrtlyrad.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gggvoirkp.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gfdzndsxa.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gdktfdkye.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gunjdyujr.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gpjuonove.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gomtpsjoj.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/ggypttlzq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/ginmeufjy.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gwbkvejkq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/ghxrovrod.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ghqgecety.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/glecdiqka.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxsehpllq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gicugcafd.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpotayutb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gdjryzsrv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/guijeflhd.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gzyielurn.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gghhgpptc.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gwxxzoyeq.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/grzfycphj.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxgauoygr.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gplzscwfr.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gxohhkanq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gimslxbfr.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gycirkruj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gotcishgh.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gesxntrdu.sHtML


<!-- 参考信息 -->