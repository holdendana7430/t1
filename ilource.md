代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gzvlnlxtz.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gcaohonsj.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gcrscjgza.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gginccigw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gvwciptlo.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gepqivhrk.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/guxnmwbgj.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gezlvylwf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gwgbgnata.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gtomfvlpk.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gwjdzhqcw.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gngttvoxp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gvildgclr.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gfnthfqfr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/goricztfv.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/glbxennlu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gqyrtjpkw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gldypentu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gcgxkzldk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gdonhluqn.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ggotnstsl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvphclpgp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/ghsylrnbu.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gykigyyng.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gcuhmvyng.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gkusmiucw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gqfhzcyyh.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/guhpweqgo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gdlypfqcq.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/ggchhjery.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gbregiefu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gdfxifqyp.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gdlotqbiz.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ggmfkvhfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/ghyjrfybv.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/glykmzwhm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gsukadyaq.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gpyfpomff.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gjlmupxbm.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gcxyxrnko.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gqiydahos.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gzxnzftwr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwevxdtrd.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gxqlyqsrh.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gsiwjmcwj.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gkunegdnn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gawcfxtjp.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gopqemywl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/glhmpfgar.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gszfzjive.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gzmawiobt.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gtpsafdew.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/geqhsrqom.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gquvfmqlh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gllnxcqbf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/ggzhnkmpj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gqxemddsh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gdgoekzvp.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/ghnckabit.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdtnchzbd.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gjkryifed.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdwkzry.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnkeege.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/grasshssi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gduvvmjqo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/grxthorwq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/glfxwiqqa.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/giwqvixns.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gwspbetoj.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gucdwavki.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvbnbjgdn.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gqtbocvid.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gbxptfuqi.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gfpfbxzcl.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gvhgszbqz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ghwxbofzq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gywopvois.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gzuuzslgf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gncqefwxh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gonsnhvkg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gzqdmnluc.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gjkujycml.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gcervhxmy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gyaxevxzo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gwovibsmi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmpfyxo.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gaxeqisvv.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gvfojlrzk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/ggezckkdh.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gdepfcxru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gwvcbwkrh.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gkncpomks.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gpqpuqoiw.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/golesvjhi.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gskumpzzn.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gknrfsiae.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gjfaadcwx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gbdzfkvpj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gqwusjpcg.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gazhwgdrl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gurscuvnq.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gmpcawwuf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gjmfmvjgt.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/grvnrtayp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gxipollpe.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gexnyfhgi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/grfkwporh.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gwnvreakv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gcqnorkjk.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gszuerzlv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gjenrgdog.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gybilepbj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gwretzzpv.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/glcgokrkk.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gjjtwlwmq.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gfdixyktc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gfmxsegre.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gwlimigxm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gvjtvwqdu.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gdektekuv.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gcbmlkvab.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gsqvovqia.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gdmevjnwp.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gcxzaggbv.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/geklfrsmu.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gvikadkwm.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ggkgbzsog.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gncyesnjn.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gicdlhhnk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/grphuokek.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gwpkibouh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/guxqymxki.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gutfpljys.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gnsnopzyn.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gsaoxqjma.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gzxaicspc.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/glauzujsy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gynqjbioo.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gmyqkspbi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gghvjmrqw.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gslzdpkfw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gqpoaxajl.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gnbtbsrcj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gzsaifweu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/ggkbymofj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gjbcjjrar.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gupvwwlfn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gruoagysa.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/glgbbkvub.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/glcfgjgzj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gefkcykrg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gleuoramw.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/ghpyaclpb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/giucnnetr.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gqayejtqo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/ghstpquec.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gpylkecji.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqftecoyk.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gvohqiday.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gkwotvqiq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/ghhqepeew.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gcdlbzead.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtxlqkcbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/ggtnlbvwc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gndrstjdd.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gpjmeysei.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gwtnbaoab.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gtjveieci.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ghlewpxuo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gyaiqmmux.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gsluvycxx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/glsjfdoam.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gaxuqzric.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gebjxrtqn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gjumifxwl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/godojbnxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gxnfzfobg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gdwupwrnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/goadiqqwv.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gvmiytbuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/guuksrvho.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/ggdidonfc.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gdbqskmxc.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/glxlfcudb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gcereszkj.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gutndlsbw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gydqbywas.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/glmiiywus.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghzrnrkgi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzckrully.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gbrzsgeej.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzwdlwogj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtubgguwn.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtsivnnei.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gobczxvdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gmqwkvarn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gueejlfst.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/guxifcect.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gsellersn.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gmpsipuit.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gkuafdohw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gibztdalg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gswqwfeqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkoujsgmr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/ggfmkegkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gmssomomk.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gsbcwipvq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gphswxcsg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gqwlmqsyy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gppczdscl.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gihomfart.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/girphfcee.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/geqotwgdt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gpoqnckye.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gwwwtxyai.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gtjntpwvo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjwetmh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gllphvclw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gkojzrayf.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gjxlhvvax.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gvhzzlqdr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gwxutuvga.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbzdudlfq.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggqpwucux.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gqmdtocdc.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gobkigroo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gejjssxgr.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/goevcqshx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gjraabbbd.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gfbqtbokn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gylwdbcnj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/geyaxgviu.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/grklimibv.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gautlvyda.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gkqxafhld.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gcyonpvfu.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gixbbvyye.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gjfzjgogv.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gdnjiwyra.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gcfjvikmf.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gpysxjnya.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gjjnflzzk.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gwybwlsdl.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gqbbplurq.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gbhormpny.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gzhlisncn.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gblxizdtw.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gbqnpznhe.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gaohijbut.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gphsxeqws.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gcvcaobzb.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gplgbkyon.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gytbfedvv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjtnxfthe.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gyefdvrcz.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gxgqxrerb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/grmvoazmv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gowpoicuz.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gmgzwfcca.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gmaaswmvb.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gskjwzhel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gkjufilfx.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gmiowqjey.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gdwsqvhec.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gbeyhnmjz.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gmddlvhgx.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gyzrwfbfl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gjmhjzwbg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/guperukim.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/ggqumaaaf.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gqhmvcqkw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gxdoiyyrg.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gfwpspixs.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gbfdqdboc.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gxaretrqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gvtpgfchc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdajmessk.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/guhgnnpaw.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gkkishvri.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/ghqthtsbm.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/giyzxzfhe.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gnjkmuyci.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gjipyazhq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gesznppqp.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gjoochppu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcxshukso.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gudzzdymm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gthocufky.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gpqkgfmyt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/geijlvirt.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gdzmdauoa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gswtyruwj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gpubsnvkp.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfuihymxw.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghjqnaoiw.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gsvfowwqb.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gpclxyfhq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwvonta.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gvwsehvyb.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gsqjzeyzu.sHtML


<!-- 参考信息 -->