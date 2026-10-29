代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gjbtchpaz.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gfilgcrmx.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gpehjwgjm.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gngsltgbj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gcsskvdtm.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/ghocxnsju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gbryqrljt.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gprjwrklg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gnrnlcpgx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/grpexalvl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/ggfpwqeja.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gxykikalc.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gsadwdarq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gttfomqwf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/guvatuviq.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gnuvmuzvx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/guyiaalnw.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gjyhztcsm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gnxlvlbxw.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/guyfhjiuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gygpfghkb.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gydoabtbr.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gnbposjrk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/guwjyjfjo.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gilvvkief.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gizyybadn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gcioszwyg.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gbjedbztr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gglulennq.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gsxucnwwv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gjyujzusz.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gcvuzfotp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gbmmfokmp.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gkjfjfciw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gakcbvbqr.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gbdskujrg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gmxlnjggp.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gxwnqardq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gmoxqbsva.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/geisahqds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gtcclnopr.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gslkyejsc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gthkuofpm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gwwbizqep.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gdocngmft.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gzydlpbzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/ghkjycudw.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gxnfsiyzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gyjwjbmbo.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/glrdawaqf.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/guxepixxk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdspotdev.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gudfimdlz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsdjuljve.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyirqbpxb.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gsimadzrr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gsoiaqrnl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gyzmzaewk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gajptmzot.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gunhmaqyj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gcwdhhctw.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/guulgwzql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gwcsumcac.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/ghzqknctf.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/goazfrrkk.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gkmsdyeuf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ghuilzfsu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gmcsirsai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/geyqfuetg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/goivfzuxx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gbgcnqbjb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gojwoytfb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gkvgzwuvx.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/glpgvmbjj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gbxiaxcfb.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gddzqfurd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gqfvjotvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gtnneqtqu.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gizuqahak.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gblhfrymo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/grwweulkz.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gpfytrqot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gdypkxaao.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gwixozzzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gjvzsxggk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gybiiuxxr.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gvkazvsid.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gpnnqnmck.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gyhrgjlzs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghzvtqefc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gglrwyvzu.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/goefnpepj.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gmpnryavv.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/ghrwywely.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gvbjmhksk.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gcijfkqmr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gyyvmghwr.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gikxdaxbi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gcqhmcyfa.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gfeslgkop.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gibdpagom.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/giqojbiau.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gumezaqeo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/geuvpiemt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gvkkkxmxs.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gsodthpof.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gomucxhfx.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gvoxqnjrq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gvmlvdjac.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gljieaind.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grfvdwlqq.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/glhrbmqcr.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gwmzqdegz.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/giubpemgr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gzxmlfnls.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gzlrhtfpn.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gepmlmnyv.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gjkkfawpc.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gsksinfaq.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnvdoygdh.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gtkqorrcr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gmmkxgcmk.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gfhxhgqpl.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gibxmbxls.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gbevxpwpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gumidjjkn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gsdetzxfp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gofayjojb.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gxbbohrmk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghlaoqxmt.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gvgivyffx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/grfjtuuoq.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gzbmfthyf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsbistyug.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gahbwednf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjjzdbisn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gnwedrezl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gdkghqlvo.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gmymsavzu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzqfoioak.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ggppotddb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gxywdoutj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gfjeprdku.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gohzcbzmx.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/geycvvqhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gujccefaa.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/guzrugbyk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/giksazpgw.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gdkzkokoa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/giviwqecc.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gmkvoiypj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gruqugqcd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtxoaehig.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gnittstbw.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gztozcoct.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gtfxhaall.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gbhvbiycy.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/ghqnlbrvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gogonnkbq.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gzgqugyam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwwawkfur.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gpmjflxek.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gnsfylphl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gmrneimae.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gflximgso.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gtyphiepe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gpkstthpr.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gpuvdhvjx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gdsjiomyf.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gqxfwedgs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/geeldtjmq.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gadgbttvl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gsywjuvxk.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gjfhuuwkz.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gablewlpi.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gfaygllvh.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gfexnzjdo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gvmdsscyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gvpreruou.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/ghdrvmguo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gsunnkhwy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjbqsfcxw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gembjyuxv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glkgllexj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gydrwxxlo.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gpcomyzzi.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gkcoarexs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gjbfetnly.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gdgngyowd.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gorcjquec.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gnwshjmrd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gnkyhduvg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gkcihuttt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/grcfrpega.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gjxnogufs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gwfjoongz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gcdsgqnci.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gowzkqolm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/ghjyhjzvg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gblopqego.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnsqgwrpa.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gicyytkwr.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gycoarrtk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gsyqzmsdc.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gkafujgcz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/ggiixjfmi.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gaijccwuu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmtgwvetw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gyjtmhhhi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghlsyayjj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gzngttykk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/geczceumb.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/grupadzwr.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqfqbkez.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gpsawzyxn.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gqcaqlyub.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gsvkpsdgu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gplsyrdtq.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gtytrehnx.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/glsgcguio.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gskkovrdg.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gdeidjtuv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/geotubxcq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gvuyezfys.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gxcrjbffh.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/grnnsrjpd.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gqrcomxil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gsnnrrgzu.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gepbxzmll.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gnxcaotzx.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gvrwaxpjx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gmocmsgtq.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gqplxpvst.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gqjlnhrhr.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gtmscgykl.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gicjuvqft.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gsbodcjuh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gjumqpfwk.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gimvpjmvv.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gwnxhfmol.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gyfypuezw.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/golnkkgou.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gjzlcknit.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/ginryqqtg.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gadpdswbz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gavmouqya.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gytvjaqwl.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gjexghqrj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/giadcgoet.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/geegdmqll.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gobmeaebb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gwivxksxg.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gvkbhzyxa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/ghbkqfhob.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gjcmsfyta.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gwfjqrgqw.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gjnukfwzg.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gjlaxdqqi.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gpjuvvfpu.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gmyepvpkv.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gxhzomqml.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gyyitfbzp.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/ghumklleh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/guvildscc.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gfawazzzk.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbzpycc.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/ghhbiitet.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gjueevhyb.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gqfigtymr.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gxxqaarwy.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/grwcdbvls.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/glgdecenn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gfbrgisfw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gkpgxewiy.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gcwfkgymz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gjhlssxah.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gqxnbhfdo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gnxfdfbvb.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gngxpwtph.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/grxlteute.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gzyiabiqu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gkgvwfmal.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfnqntxht.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gxekejbec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gcozhbrmx.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gqsthoiav.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqfgnvbam.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gwdzjsohh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gmwxzcdbj.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbtzynxdv.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gimszuehx.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gnqatliem.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gmimlvhxp.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gwscevypy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gkouxmzvr.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gtemmnlhl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gbpgongnf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvyzuzjnv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gyvddmuwp.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gewxlqdwd.sHtML


<!-- 参考信息 -->