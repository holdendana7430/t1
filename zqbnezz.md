代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzozvqzxa.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajssawh.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqulrzlxg.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gipywpuwz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gdayljxct.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhiindf.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gblofajzu.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gxwjntlaz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gihofzqpz.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gapbmexqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gpvftzarj.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gylcnsqdp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnsyxsts.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyfhtxhi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsneqzkb.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjumofalj.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gzncmkeqm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbcryve.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gacrhxogr.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjosncjgs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkyqkhdc.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/guihxrzed.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gylmjsbcz.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaooqkucl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcaupwtu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcanhdfan.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjdrrtigo.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuhsepjd.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpydydlvf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwedasca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyncbfbwh.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgbucmua.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/geaahcuah.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gyytuncpy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gisxzzkkz.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiktnygx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotgyqwnu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giypxavnm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyatdzjdr.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmhwirggf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gucieknyz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gsvdkumuk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedhfxlsp.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfgdbzyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovgxlvp.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/glkegnzke.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyusudhh.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gxoyonkbe.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdmnyrlp.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gmznsybry.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gufrdvqid.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyolxtzl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzeiazqzd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gpqsieltw.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gadfhfuej.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gquoljzuz.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gtalqsjdc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gubqfnjqb.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsipgmuir.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnlfbtev.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gltyykftd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmwlnyzzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmmrbpwc.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpalaovx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzliyqfmn.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gaolmfbku.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkrfprqv.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggamlptyk.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glhmsssnh.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvxhynlel.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxyyykqk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtexvwam.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gdqcqoepq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gdwkgxcoh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gdjpozgxh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gccgvrxhv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufqikph.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gsowfzpjq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ginzyjgry.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzaqdqwbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gbnarwpbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gygvnclck.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/genmydnjh.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxczmpebf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiezphrx.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsgyptqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gscqvkdok.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgqyazb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gnsiglmij.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfevyjpz.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gebusptvn.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gchyrkenq.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gennmsmtk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqowaaeca.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvjpjczx.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvblrumsr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgomyxrt.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugmybnob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gelxgyynp.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrjdrddu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaionspz.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyynjdyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeqvzkhp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmazvpjxj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkrumlaw.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyimwivxz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmwbohoe.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpdvjdqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtgpwdp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfafgzrqh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoodwjqq.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhebbkdn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvpjoyav.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqlbdxxc.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gfeefdgjo.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdmkfpiz.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gljxesnxd.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gejnguuox.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gzflkjlpx.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdzmdnlx.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gesvsduur.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gyhiuojlr.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvguapg.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzymwjfd.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gfqbuxagn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxylivxm.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrectfto.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdqiqcpo.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjfvvmmg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbmhudbie.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gimirmlxi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwhhkxft.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgcbcnzp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefodjhyg.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gomhgdpww.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvuxzaykj.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfhiufdy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/guzqxtoxo.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyvzkvho.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhzirniv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gklmrgxpa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gmwzvtkcy.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gowevrjfd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpleykhth.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghvoziaad.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkfgcxdka.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqrhvsjrh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gunfcldvo.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gvecjlfie.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtfcmrlb.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gddiofiyo.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbyflhtxs.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhicnabp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/genxvltab.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdluwfbkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gznhuwlic.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gimlpcheu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtbyvrzp.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gficnqxdy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gvayhxacd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwyvbcofg.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gilnyuhey.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gksmsteyb.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gvsdypgdq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcztlsehw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrnepmk.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gnjxbltbg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gvlcdaqzf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnvuwinza.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gczkdtwmt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijblqnwg.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gyvelslhm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuxrgrpj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gqftipwkw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gppwusdyh.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gijktrdru.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjapwafnv.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwrrzkubv.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyounmnzp.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/grdoslgnx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnovknml.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/genpukkkq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwiiugzt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnehomzg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahxnblye.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzylbpqzt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnegqggh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gecjrxaze.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcabrepoa.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/guozgypqo.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsijijmzj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/ghklekdum.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuenuotq.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gxlcwzmxa.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gfstaufsn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gyynfmbjz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gnrkbvwbd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrpbfdq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gnqfbuqih.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdqrkllw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/giginqlwx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/glilckmno.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gyajkfxwp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gvipcwssl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmvhxtnku.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gvzowjdxd.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfqflxxqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzppjzrpk.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfsoubzc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdroswcfg.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzphhdkn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnwoeetwi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gfnvuvtli.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvvchjyo.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxpxakqs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklgmrzen.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzaubrwb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/geygqdgdz.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqfizpmb.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdxgtoqjc.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gblmihpdt.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grmcruwnj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtkgchow.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gqtkwuqkf.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzaijkxio.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjjzxyoa.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuxxsvxv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gxflgfkwr.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhstyzkx.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbwdpohf.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjnpklgcn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzeqnsca.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gphyszmmh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gunaewuvk.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbfuczvo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/guirlijlk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbbhvcew.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gpcpwxepq.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gquhoxewz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnqdfuv.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gmnnellee.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdimfvxxu.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gteayegez.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/geuegfkns.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzipnvs.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gtmcuvfph.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gtlxpvzhz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvzaygur.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqbdcerx.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gadfcwfmx.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/guhxqahnd.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxegchgip.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gicxgqwrr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlfrwyig.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gkehlslaj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtwcfurf.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gpkgfobvn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvtnjszw.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gajlahdaj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gkutrfqoo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnymzwtm.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkxmyqafo.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxumfjjln.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbwtked.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbxqtxmg.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gvgwwxkyc.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gxrtiirca.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gficrfsgw.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpksfiwub.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwuyycpk.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzdfjwrw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/grmphibcz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwmzrlze.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjygyuaf.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/guuyllolg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guojmzspg.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gareyxvrj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoygvmnr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglqrbtem.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gekghkwsa.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbhyvnrc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfkxmimr.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmtxkscfk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlcgyxes.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/galucxxrn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gctfxxbqf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxgzyinv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gfdzjbbdt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtdpivkk.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfluyoywy.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzyjvur.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpouxnhrz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeucqcwy.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirbdipe.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcfsujlx.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmfrxba.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdatlmzhj.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzusnsxua.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjlhnnhk.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkizgire.sHtML


<!-- 参考信息 -->