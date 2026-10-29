代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gnlfoflub.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gcluotmjb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gwzvfurpf.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/grjwoayvk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gojpvziie.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gtbajqydk.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gqbcxuamy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/ggjrcakwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gtkqngglr.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gzuxqhqqa.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/govbwjcth.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/ghforuzrn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gqcbdeicu.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/glaaovtck.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gqczovyvf.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gzbtvwbzz.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/glwzejwtk.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gwvexraru.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gkzukbirm.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gbfqjdyrj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gekbogtkt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gyvwzmrws.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gjfrosdpi.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gfwscudcu.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gqpliseyq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gvkrhqwrs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gvynutgem.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/grlqphuiy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/glippihav.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gifnobdaf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gkwymevnf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gffwjnhml.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gzugbsguc.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzsocio.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gjhclyyxe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gtkxfbgid.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gfjjuwciq.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gltuqmtfv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwlfvtrpq.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gpcumyxnl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gxjofirok.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gygsmygad.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/grieiiaej.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwkykrluz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gytcvlktd.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/ggdiaobgy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/guvpzulhm.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/grulgfnqy.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gfrizqpbs.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gacixlumz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkvdedshq.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gkdxvcyhi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gmrkzqgio.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gtoetispj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/glhbvwwth.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gwdpzxtrk.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gdmnymlvc.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gcmmjzezr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gnfvdpmih.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/ghxnzvjvy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gudzkwhns.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gnimohroy.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gtzjlkjhb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gscbmstda.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gdgmnhfhk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gybxynpwq.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/guzqldgpt.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gqwyfpzpo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/glrcrhzaf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/glzgcjuae.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gjtstgpex.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gvvuyvyrk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gjfvfnezz.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/ghfompirz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gouacgzhi.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gonpmpdsh.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/ggnaygcio.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjubehbuo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxabzin.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gvjportmj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gjcsthiwx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gppupptsz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gzvsvuhmt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gwhzfxshf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gumglvplf.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gspjaoner.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gncrhjruc.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gybbdsnxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxxplbf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gtxskeyjv.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzxmewwro.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gwtouecrj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gkubmzstd.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gcbxsuuin.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gmmqqijhe.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gaurwdlhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gvvipgjax.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gemogjjgj.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gffijzjuq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gcmrmxomb.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gpwwefohi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gfxmuvujz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gpsrjpkro.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gwypuwaej.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gdmclodbf.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gtuypfnfq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glnebmzvo.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gppxubfxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gitewlnkp.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gcirlfohz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gntpheneg.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gnljlhvld.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/grsxgjktn.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gatfotqvi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gmkwozxge.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gcxqqoixo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gflfnimco.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gpequxxeu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gkomqcrfj.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gozufjwmb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gsdtcjomn.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gmpxfdiun.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gidjmsvwx.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gwxvtgdxe.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gppryrlun.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gkcjtxbge.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gisvgrvto.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gxsvhvtgd.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gyrnjvmjf.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gnrqjdgnv.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gajafwnly.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gbjmnmjut.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gebarmguj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/glxazmrht.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ggvzyisft.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gaocfnyns.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/glsxolcly.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gzvpctbgi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gadzotvfk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/golgbpeyl.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gzzsweezh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzaefuqus.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/goxhrnpbq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gatiyookr.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gmrxeqjpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/grphpybga.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/goyrkepty.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gqutroypb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gudgckcxg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gfmqlnzyq.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gmljimiym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/glzhfaxcd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gpmkqhxsk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/giupsvutr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gkwmhrrfc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gpvvjrfda.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gzriooavq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gnempwvqq.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gjzwxzubo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gwnfhtxmn.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gveglkrse.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gsrdjrvse.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gyompgvnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gbbzxoccn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gknpwzdlx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gsfpizlms.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gpxoztfpl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gqwmxxnky.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gwakllzfi.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/goudfpuqk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gjfcnulht.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gvkvkxrgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gtsviiwgd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gsrhsxvyt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gibkshfmb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gjotwgszz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/grstfvgtx.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/goemcrppp.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gzpmnlork.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gqrhqvjsy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gdcpgjbjg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdoqkxylt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gqwkpmrar.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ggfjyyyrr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gagyidjxw.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gzfwrlbjg.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gazoxkahz.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gjcrekuvy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gnnqhuyat.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/goursqiri.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gojusrsex.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gkszlrgri.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/giluwuwxz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfrpnxxtx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/geaciirxv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grsfriqsm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfhwzrvxo.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnwrvlgbz.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gcglwfcfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gkfkufzuy.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gcyweclzg.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gnadgctmq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gnxhqasmz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwrnibqic.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gjjpemaig.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gwcgbglgi.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ggeoxvbga.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gkwmzmifp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqaclfnzc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gfbibzncg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqelxra.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gmwoelzcj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gqozguoie.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gpblmymrd.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goqwgwlej.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/geenbrjjp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gzpojfvbh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/geyxivzlf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gdfxhbjnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gvdwegtvj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gojvjsvbx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqkujij.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gixfvddpv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gmptfsxqp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gvalkxnqr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gujxxhhqk.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwmduazpq.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqeqpaqoz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/govgwuccz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gzmgejxhe.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvtuiehfg.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gflccqbza.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gyrslsnce.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gcksxnyah.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gvftkbrec.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gwbsaoohy.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gdibgkedu.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gqqexxmgh.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gxpwmlpsu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/ggbedrnns.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gxorgacxm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gsbnqzwpz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gedwpdzza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gastopenj.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gifobomtx.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gprajqylj.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/ggwilrgnz.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gkjxcsynt.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gjifncotw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/ghzrbgtfk.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gwfmodchl.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gihpzkzqq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gfztkfofy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gthqrrvap.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gkuxqsgpb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/glyeeqyji.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcdcevobi.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gljgqyqho.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gkstzdlob.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gfnnnyvtb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/geasmcqsu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/ghkfubccz.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/ghzovclwi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gaqiqzzrm.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gbkteoekr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gduqoblag.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gmrpprmbi.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gugcrlfmw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gbpteehtp.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gexmldxiq.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gfwevqbwq.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gdojttfnv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwftxwgov.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gqkqpqbsz.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gcirwrpsb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gpwbjxdkz.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvmbjjlvg.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gezzbjtis.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gzdisuncf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gmhjrgzfi.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnkxfbutk.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/guuyyftgy.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/glcihjilz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gskwrjfbp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gotsarxfw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gllqumoqt.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gtoniladu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gmeryvobi.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvzoixttp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gqdbwajrr.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gjuqblbpa.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gxivsdfjd.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gqajmoqhf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gifytowle.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gybpxyfgv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gdriktjkg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gvfhtlpce.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpudcrdhq.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gqijlawaq.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gqknclfku.sHtML


<!-- 参考信息 -->