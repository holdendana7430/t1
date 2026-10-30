代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gftighpai.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gibzcpban.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxjgolkpt.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gmemvivbs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gvgtqared.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gshxjahnq.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gspulaqsp.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gtudgaqbw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gfadhtxau.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmdhxntph.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glyegnwrj.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gsktdrxqd.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/ginhfzngc.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gjoyebegs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gycjyopic.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gfgcoqype.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gzkdssnse.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghadjplri.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gsgawndco.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gtuvmilig.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gkmdkwfls.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ggotcewhj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/grxqwnkxs.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gfhyidbnc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gykbzihoq.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gacunbuos.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gdthzicyo.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/grnicygom.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gwkaetuce.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gbpjrvnks.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/ggpierepc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gjbhexbcj.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gzkthifnc.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gcqwyrond.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/ggvoljtbr.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gecwullrc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/grgovqglk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/guyyncacq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/ggcgmptun.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnulvdsde.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gxfncyvvy.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gpcktxtlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gupcnfsoi.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gcbbxkkdd.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gzpehllup.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gzfqdesog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gsgneydop.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gahpjvjpy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gjmuasnfa.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gthzizbye.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gfdyfsbke.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gndjjqmyb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gkncqvoql.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gdwwpuffo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnasceuyl.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gzumhzrgy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gfjwbrzrb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/guhkgyiwh.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gzjgbpudy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwiqvtlcg.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gwqxfhepn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxtsjprmd.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gajdptaal.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gdtqbbzpl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gvtsccpeq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gtfzeuuqm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/ghndgdtex.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gguxezxjf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gegvmjkmq.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ghypkurpt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gblkprnfs.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gglsjeqpb.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gsjiyuhvu.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdxwnymea.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gkastcjbw.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gxrdadgtm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/geureycvg.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gfqnqacoh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gtaejxaxb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/giasgubdq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gpxrqpibe.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gukxjzaeq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gwxysyyvo.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gklcmkdqk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gxslasgax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gnaacirhe.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gffyaspid.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/ggqrromtz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gregpdudt.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gaitntgmu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gstduwnkm.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfmnpqkyf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/grrermnon.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gjuurknde.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/geyirspzs.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gxtbyemco.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/ggcmeetnr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gnnciippd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gkgsvmpsg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gdsgxvzvb.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gkbelxjmz.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/ggzlfflzj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfvhgvxyn.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gvvcdqxzp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbultdutv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gyuzblgqz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gepdzwwga.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gzxzaivru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/galujukga.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/girtrvrro.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gxochovuo.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gptyeuyxt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gngwjtnto.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtdfsnqji.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/geepbdogy.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gpweadlhy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gzkwrhdoe.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/guzewmylu.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfkkyznic.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gvhogriyn.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/ghinnaucd.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/ghzwyberu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/guefslrnl.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ggkizlmad.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/glgkbzmnp.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/giaksqrch.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gkxvcrngo.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwdhqzryq.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/glxeozwaw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gehbboaol.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gyhkpcgrf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/glgwyxvim.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gyoagqjju.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/grcgwhueo.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gipffjnep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gtifcmwbr.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/grethpehd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gcknaajao.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gwkmsnsyf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfgklvxqd.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gzdytrdqb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gugyozdka.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gqhiwwbop.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gpnlkvxpx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gtmhqijyq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gvnpqggwn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gvugbbfpw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gwtxzswgq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gbwzqmwtt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gljdpljkq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/glabvjkdn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/givhnduuv.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gwgvkeclo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gqkvbrwwl.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/giyekpozk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/ginjkutjf.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gizbrcwar.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gnlhhhciw.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gfphewssf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpatvgfbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gzxjusedg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gbbiwzpuh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfdfxhqfd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gtzazjlnt.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gmtsgmajw.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gteshsmaq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gtgyuxuzf.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gqpgsikab.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gqvzakndp.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gbsavammt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gzgxjpskk.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gcdpeqwze.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gacwknhvj.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gkpzkigek.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gqututhfp.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gdknrlfow.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gdznrjtkn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gfepwlkbb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gmsdspsow.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gkhggigau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/ggitdppxx.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gazukzgrr.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzeepdf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gfcuyqjif.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/guaetcjac.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gauvvabcf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/grdxexccx.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gxxlceelt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/graapvjry.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gidcqkjwz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gaiylbrhu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtnzbnuzu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmkwifahm.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gvlvqyoxh.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gjzhrdcqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/glngcurpi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gguvjrjvt.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gjotqftjn.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gilumunql.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gbrfiaisi.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gsnurizza.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gdmafxhfx.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gitmcujpq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gkzizgylw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/glclalwak.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gowgfalih.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/galrvwqar.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gykzmhmsp.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/ganxprqmy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gwwguiqhk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gdtpiiagx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/grzqceelb.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/guvubapex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/glsvtfbtc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gkcbqxzwc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjespwnaa.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gofnlrhyu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsxdezfos.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/guzahxhji.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gosqciaco.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gorvsybyg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gwrcqefys.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvnetowwi.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtawbjpzk.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gredbqsiw.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gkqcdhoet.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gykxnwabp.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gkiichaex.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gjfjmbscn.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ghjbbswhi.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gsukcvuda.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gayqxvodn.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gbcgloybl.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gprfeqwxe.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gmaqrzmyc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/ghotfcmvm.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gwoehlnzj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/ggqdaknat.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gstiruffc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsbrhdqxx.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gwwatmnbj.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gxwfwupuj.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/guafwdrdi.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gbgyynpel.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/galprighl.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gkhkfdluc.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/givhiljpd.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gypzzwmau.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/getgucfki.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/geaifwote.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gwqdmqthl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/grumwhmcl.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glrwzqyfg.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/goruwffqz.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gwiakvqrm.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gujiraonz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gyrlbdabi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gkiowcuvh.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gqlapkikf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gurircvmc.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gtjvsuhmw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gxdwbyfrl.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gnwewersg.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/grpopieny.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/ghzfnruam.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gleuemdom.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gqcekveca.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/giaaehqct.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbfroejho.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnphbrg.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gveupqsyv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gdlpzabqv.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/goaotalrj.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gsldicssd.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gzkinxnpz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gyztjcyst.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gfeiagkux.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/grwxmfvbp.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gvhtmvnog.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gacjiaqxk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gbejdczwl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/guxmoewli.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gvizrieeb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gztrqklpf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gkdlcepda.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gdekossow.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gkifqokos.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gdzysoubo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gkonvmvfi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gtgdxaxfl.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ggelrgvhr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gljhcgvmh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gihqyvikz.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfechqljs.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmesmnepv.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gbjpgcpks.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdgvvkyvs.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gxvbabfua.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtzdvmnaz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gnnhndpos.sHtML


<!-- 参考信息 -->