代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtuuvsdzu.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gixmwbrfd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giucclaag.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtrxoycx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ggxwknjwu.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzypqqjc.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gywuhukmc.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthuilarg.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gcbcyfxbt.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbhtecybi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/ghorioijz.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gdolumivr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwchvgey.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/guhxgvqzf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/geoywteck.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvcccklg.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttdnvrjv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoiaihag.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkniltkf.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpabrdncs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gkphdzyte.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfjvuiow.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/glaztvttd.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqfsgbpi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqfasjfu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmbbtavj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfbsqyu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geafmidsy.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gjffgmaaz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gqdgzzgai.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqkavqcwu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gympezonq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdktfgaq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwwczrgr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gysenhubo.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfqjjbyrq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcijhfed.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdxobsj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggubcxffe.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxsfhbjd.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhrgncm.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxnsmtla.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyjzdsrn.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/grkqigleu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gouaugdyl.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/garijoaxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtraduzr.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysfxwpcv.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gyipsrfuw.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/ggyidimei.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaywvajzj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyxqazfo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtipqietl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gajoyzzmf.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxcsjdc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gupjrzbns.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnoqgxfy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guxlntbok.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghtpltumc.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpxpkqll.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcabgtqtj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghardgnkk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyypyesq.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggncisbdd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrixvkbr.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gikvjjpoq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsjzhfnw.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpatixvxh.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/godakmeko.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdiaafe.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gzdbryfyo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxmobgkr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtnhcuft.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhxcrqdx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/glxltxyax.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpjfiduc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gepctlpgj.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/glrxnbwdx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gvxavcsib.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmltmbthz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/ghhjwpvex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gifzwplbb.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgdlpcsx.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmapmovun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glfagqjfk.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkkqhmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvrhazwx.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/goqjuafpm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxpcwonz.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtuseecoz.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwujcjdmn.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmbxgjty.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guekjzuou.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdfifsib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvuqndeh.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfaxqqag.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gegwkvplc.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzatbydsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxpevfxz.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gnchgoetp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfiavxqe.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gshpwmdsw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvjpndgr.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gytvtltgm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gqanaiaqv.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gwmomlqmr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtinwngpu.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtoszazvu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gadnybchq.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grydvnisi.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gwfpigggw.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrkjuran.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gomownmwp.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gyyxzuban.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrmftqne.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtndrreye.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbwdzmre.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjucauqmm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gihpijpue.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxsizxhd.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsnfeipa.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqwkujd.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gifwhulwe.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnldeylt.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/geajfjiyx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpikgntwl.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmzsocmca.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/giynnernb.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/geqzeajef.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmgnykwz.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gseegetpo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwexvntit.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/grgdbfvpw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrdmursj.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/geepipghy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdswycgg.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/guotdgljm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotgnhnuw.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvofkpitc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ggyvmxvcr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkiuhecu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/grrmokclb.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvwproimn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnmyttnp.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjyjhjzld.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgdvznzl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gaanemxol.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjuunypqb.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gaxvjijhb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gscghjojh.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gbsvkutym.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gogmcchbj.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gbooljggp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxfmupjs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndwrfloh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbrfthay.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghyecwicc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfayzjiu.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghgrsyqqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gjineatid.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gundyikqa.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaamuwjsw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzztwtdl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplyoxvg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwcqewh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsxhdece.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gogssxwnk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrxeglhs.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkvflfhp.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gwaokmnwb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gdhfinusv.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdybsqmds.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gskmrrzme.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gdqrmlphz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gegmpfavt.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gcapvltrr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grlevwdzf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbquujus.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gssuzvbbw.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfjayvde.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggizokhhe.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gbjofrxlh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyqmksyg.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoyfdibf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gaxtosgmk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbzdlfjw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqncetfh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdttttvfi.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwkmzcnu.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpiwmhva.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyymsamyq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gylhmhogg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfukeshn.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gosnxoefy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxpmfhwa.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsedbnrq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gijuistki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gngatvgar.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gdkakcyiw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasjvlfkw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gufrzucxx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjemzxrur.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gytpzxjml.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/guqexhtvn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxbpichuy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciplsnzi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzbtkvf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gygxfahod.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/ghkblwhnk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrhlflrr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/glfnqnqvq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqeftjnzb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdizhtku.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjceetfpt.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/greoauazz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvshgmjn.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxbsmgoud.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdavztjyp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvhugbj.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsewkxtmo.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gcgphakqw.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbcgkcdx.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmcisuclt.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gpeqtxibh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gylwysacz.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gepsmsikm.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspfihyco.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwamszba.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbboedar.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/goynfgcmd.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqsvdkoc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggbjeiacz.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gogfwvdew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrpqhval.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gaiyuapnp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdraomxgw.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gwpdtyduo.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdvxwrnn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaceahtyy.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gdginduop.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpjumvsjv.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfcbawte.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gpegjofjg.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gezjsmztq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gqffhfhjy.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/grclwirar.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/godtknjnb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsnrlppe.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzusmhrgx.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagbzuree.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmtwrzcee.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gymoqcjrl.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepolgkmr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwkfnymz.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/grceimrbe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gotfpdijz.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqidddph.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gucxdgljn.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmoulvfop.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gnrysvoev.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gltlmthzt.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/guwukblur.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwekniqgn.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwqmvkhv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkoopaun.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxrqrxvj.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gihruhefm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gzzgrwwiu.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhhxcnhr.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gczmzavka.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhfeqiiy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gckdlmidn.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsefovxzz.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gexynpwbl.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxyaasqy.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gszjyedxh.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gagdmgpxl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkxgalt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gbudczgff.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqakmdqk.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gkotnmhad.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwoipirgj.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/guxzztmuh.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcsgvvhh.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtvsxxav.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gitimuoad.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzxiiaqrw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gujpfjnng.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtmkmjzd.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxpypmm.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggztsnnuo.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqzzcmhx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytzxdccd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gngitaqqq.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gcxwoktfq.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gddvorady.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnyxlmvo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/guxewuidb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjqbdvjf.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gbqzmoaqh.sHtML


<!-- 参考信息 -->