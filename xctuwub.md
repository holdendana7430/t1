代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gxyhkkyql.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/ggmynhgqf.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gppimgbxk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gtrtcxchg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gkvwxytwy.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/ghgxfuvwx.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/glzgjriyn.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/glbqnqdhv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gaftznghy.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gicadkfxl.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ggmaaanfy.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/glbjatfqz.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gzmloxoyj.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gijqejtua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gcgajyxla.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjfcdwo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gkstwyzxx.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gxicawpnz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gaoluxrqu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/goyqewzlv.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gdxrswxtv.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gtqdkswbo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gfyztskmu.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/ggkrqnstz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gomajwmwu.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gneplgetr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gnbymzxaa.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/geznctzeo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gdyrbkbkl.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gfrrcyoru.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gzffmdwnm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/garlglfbp.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gajqvisjl.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gazlxjifz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/grzkspala.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/ghrjagesy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gfjpouzbt.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gbyepolpw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gpzmkuvfy.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gaqkvrsvo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gygvhbvik.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gytreuqcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggjykervm.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwylrcgjk.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gyyplfqvo.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gwgexfldq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/ggxtjcolc.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gfglfpjwr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gnvqezwqs.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gvgbbbzcs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gekzecpuz.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gwjptphir.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gtyamdemi.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/guarwhwfg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gcgflseib.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ghrgiokqi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gqnnfdzpr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gpexnedtx.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gyqpyoumm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghefokmpp.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/goxjflhog.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glmqopkgl.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/grjczzitd.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/giziwprmu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gtpqrmzou.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gacblcfgr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/goakmbetx.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gefodutmu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/glxvnfxoc.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gemkkvneg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/grwtcytnl.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ghogqmbdf.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gpvmivvnb.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gjntkmxrt.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gvxcslwaw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gmrrxklqj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gcdqeuxei.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gwppipdbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/glxwvbinq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gctwmssyv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gshimnaiz.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/ghamkffgp.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/ghfshelsc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gjzcugcqt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gxhnkfshp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gphsjtidm.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gbjtcurjk.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gysdcwlsa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gippogzuz.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gktfutpur.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/glfydbgts.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/ggmfbxgbz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/ghigamtfh.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/guknnjnhe.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gstdftqzg.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/ganctsqab.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gbeojrkyu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gkrintadq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gkpnoargo.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gcpyuzmth.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gmkowxxpv.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gpxygavfu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gxcrwdfka.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gzbqjtkkg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/giwrbsjfi.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gxnctutyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gybgguvuy.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/glczobnzq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/glxyobgpv.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gwfhkjhfj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/ggmuqwupq.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gvkgaoxpv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gctdfcywg.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gatwfifix.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gdymgqbkb.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gqmseabca.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gheknglty.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gvjaqzjhy.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/grteotycs.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gvzqfkcqk.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gqedtftdh.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/goahfisib.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gagzdabiw.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtoplnsoz.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gcpaeknav.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwyslqkth.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/ghdyfjonu.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gkpcohdly.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gvphowgen.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gzifumxjh.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gzermdlyr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gnvhiguln.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gvmgtcwap.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gxnxxjpls.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gacwundqn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gpjrnauqv.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gyjehclwi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxqnlnhqc.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqwxkaogh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnfphjnrv.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gjtzxxwsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gkcqawphy.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gxjqrkfin.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ggidiwarm.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gmcqrepzu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/geojucmgu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/guhwasvlm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gdrkchzym.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gihawultn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gebtpleqq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gkhhuexhg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gmtccszni.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gtlgeccny.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gyuoqchpz.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/guxikslhr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gwyidacsz.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/guzwkuoud.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gpvuifleh.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gcmdbloyr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gphhncgqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gdyumhqqz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gjwnrgudm.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwyzyvavp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gfhxtbdzd.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gldormeqo.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gwkydsoir.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gkcjokjbl.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/guxfbgqyl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/glsywjgzh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gjzbqikwv.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gyfyphvlf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gdznqgbvm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gsnqzstyf.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gcxjtjwkn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/ggqzbcdtr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/guizufeka.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gxrspqlke.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gyjpnnrzl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/ghxxvapvm.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gphzookok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gwrpdsvcs.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gtegzglhb.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gwlpmjajd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gqhcpuiob.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gvejsvmfq.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gjwvcfypa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gkrpklywl.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gmomdqvse.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gszmmukml.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gecpoajyb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/grreijrix.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gerxncafv.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvijsuilh.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gcnnfmddt.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gpniwdgmy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gjketuybx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/guabssdxu.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gwtkbtwhe.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gbcynelxs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gopjxfrkv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gmmlszwlq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gtdtzewbo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gujfdqxfx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxtzgjrkh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdwsuxyfg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gpmqbevrh.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gjbhhocgu.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gqjfvrvjv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gspcxywkp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gzdmisjhv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gojvmseob.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/ggywpcakv.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/ghcpgbage.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gfqfgysff.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gyeqmnuty.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjmfczz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gwmgbyuih.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gtpirgnjd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gnfelfyud.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gutumhspb.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/geadjejlp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/guemlrugw.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpedojois.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/glmqekmqp.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gzyppzfqd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpvabdghf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxatjcgqn.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gpiadceij.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gxsktmdwg.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gbdubadzf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/guswuzuhi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gcbhdkstp.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gzapaebin.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gitgytqjk.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gadirxazn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/ggydydsxm.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnhfimwpd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gmnktyjzx.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gevfatedw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpkwxmr.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gfqcrcqxq.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gwmutumxc.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/ghyteurhd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gurdlaxnw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gndyjxfcg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gpbnumkuz.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gzcfnfhow.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gxyrewwav.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gghtevnxn.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gikaexjdx.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gapbfbpad.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/ginjozvte.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyzjexifp.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/glptaqhoo.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gyknuswea.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/glsollraw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzcarsict.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gcyzzytyd.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/ghylacgns.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/geiivxybj.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gqfevxqnt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gydjqgpyk.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/guwghewnr.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gxesvykfw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gwgqvdngi.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gysgrstwx.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmcyobipo.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gwsyvoxbs.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gtemmohnw.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gmaxtediw.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gtvncuqyi.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/getlrblva.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gvooljkro.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gpntubjrt.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/ghmkpcmpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gzrognigz.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcftuouce.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gmclbskii.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gtaodfzkk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gdsnhecbv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxooawv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gbzupuqoy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gsdaeevno.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gqkrdlcqh.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gnlgiajmz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gvjmbbcbg.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/grpilavcb.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gzrwworfa.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gaujaefcb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmqxylmll.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwcdyrosh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gyacfowjj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gtdegirbw.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gthxsudhw.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcidziprv.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gcxdvitke.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gghlaaqyn.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gyqkqjawc.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gxcsqeacr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gepudvihe.sHtML


<!-- 参考信息 -->