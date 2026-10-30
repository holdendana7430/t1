代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbkabytb.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdhnioid.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqkntbkk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndzzwhuc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/geybauclc.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grakdamgp.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjgoxuuij.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gdvyfzqlg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcvzfohm.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grizlqwvd.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbppvtcao.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkocnuam.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/glotseage.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhqvyuuk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcfiaeci.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gdkhbkagn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gctzvwlsg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gtttmpsjr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabsmvrwl.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gjnckkgvx.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyqccfzs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcrdrwp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvhzavx.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gurpmykzc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gprecsmlb.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnkyzurdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyagfwhu.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmisjynip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrerbzow.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpffwgab.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcsvlcxo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjoufdsu.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gujitvart.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjoudayv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesskqzlj.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqvagxgv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydeeecxa.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmeeaciyt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfffmdjq.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gokksyidy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gxsovewfk.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gxxrtcojd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjbdwoll.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqzipduc.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrbljcfq.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/girwtfyus.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuxoxcgr.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuweghui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gccrxtrzm.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcgiqvud.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqoyyeaq.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/glezkvnbq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydguvqys.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjoylsum.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggauifikl.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gyypcwtnl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgtsbiwr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvjkoonz.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtqhchcd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwsmbnvr.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxovxsohh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gybxnxrcd.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmdlhmlw.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gtfcndngr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihxmhbip.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gcsxawhzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ghddbsjkj.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gepncwtrn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gldbnejgt.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gjfrxdxnc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gwyckbhem.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgugjxhh.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geajhlilp.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghdotusms.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gkpyaephq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gadrherrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/ghastskqw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwwhjfkq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowhsxkfl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gaczpayzp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/grbpahvsb.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggknhlese.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqenqshp.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gygjkoiex.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gzkecpeqx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcnvooho.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxskxtsa.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guyuqoqod.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaegawxjh.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrmjooda.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gtrdgzxfm.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmwdzjms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gnvdkcxal.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/goclfvuyb.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gjwffadpx.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gbaaoaumv.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/goqngowxh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsxtdslt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxbxlmvd.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/guigeeyoe.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gslvvjmvh.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gatcfabti.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grigiexyg.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjqwiyzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzlsauzop.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gwlvafrbb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpsumdsa.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gymbcbkwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwawtbcfh.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/guvxjlwok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbahxlzuk.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gzmdakbxe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcxrkcxf.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gycckzlyp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnpywxb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzgvrzy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrhrypz.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakvpbjdo.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcapdvj.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gooyffsrl.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gyvivewra.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/goeghkozx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gqygtatuy.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgtbducu.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gywhimqzs.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ggurnwaaa.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvcuewdj.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gabeptlcy.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glkfqislm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedsnsemx.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glnqdzwae.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihudaxe.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbywnueu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/geillgyet.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgddfucg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnstbiekf.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gbaavcfrs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxsxambc.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gslfrcgrj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaijhlmm.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gkydngjyq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gseqbypld.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gtddftehl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuaukbor.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtfwtooy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/goxlonyju.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsmljogp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxpjcbf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grpscfibb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbgsljnc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfhaqcfdk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gofjuibue.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gddrcithe.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyypxrbu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gtpambevc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gokcvwggz.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/grljjgehw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmmiavmme.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gysvdrbvr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gusemjrgl.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gdyldoejb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdvyzbrlh.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gajowlqtx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyfbwfsu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonjckjwg.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsdkqdwpr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthhgahc.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggyejwsmv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnpnuwpb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqvraklf.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoedfiyw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxctvae.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqzlwiqm.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gbplvjgnp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsykcstzf.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjumjdmoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gzaahlmyn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstrhgdbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gwggpkzma.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzeetujx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gurkitemm.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpxloay.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmujadcd.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccdydggt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzgekrmu.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyizxmon.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsejrrrjb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gtauizlzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/guemrtxxj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwqyfnvi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwmlpkq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtqntmamx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghntzalca.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwfdthzyq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrfibtfb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/ginkhbcgo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuxbjokn.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcogmijdr.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ghrssjxff.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gwhbceukn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcdpzmylj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssggfpjz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyxdjgqw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gpwhopvzb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gnheknaki.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gffbvxzkj.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gfxoagihf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztocggha.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmmlekkjg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyanncrlq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfcmtlzp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbarhiaip.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzjeepph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/glzccqzaa.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybxqvyui.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsufxlzqn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrxanpgg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklmoxkmm.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxgfqnfq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfiaqeay.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gagdgxkax.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guutxtbzi.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmueprztm.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gglpblnkw.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gdxtjxneq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvtfpcrgn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvgefldc.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkhmrsgr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/greesvjqh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoruauhy.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gemdltakp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkiutpbj.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfgfvzbn.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqkxbpfg.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxirhbrz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/guwctyrjw.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnpbercub.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/guoaodaip.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgbfecnc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkyeckfnb.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/ghxhcqwad.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcngtlmgd.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbkcswrz.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gajycwvvg.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwfojcr.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpiwykeq.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxzinrmui.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gabijubdg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxvlyxp.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gllvrtnlt.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyjycwt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfqqrrlp.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoxcvqdu.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdmxvlvz.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvdlnsvof.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gylyrxrky.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyidhuyr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gatsvrlpd.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhrjeir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gewsawrxc.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gihvildef.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gftuphnbq.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmwwbymw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhluhhxc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxuviidh.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnxoxmoqn.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gswsqyndf.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gspjlxtuh.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glqzoxjsk.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyztvjaln.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gjfyeudwt.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gjhgvugyn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grznlybto.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrnhzopt.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/guchspuqx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtepufb.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadqizimh.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbbduzqi.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwenmyat.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gylgdqerv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmudcdyp.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzqdzbnry.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gqodscumv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtlqkkao.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gnsvgyfsy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/govmugjyk.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfonamh.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmebafpiu.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtkjvcsks.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/grjebkyhm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grelvzelg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gzhsuorao.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gulxkmwes.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gukxdhion.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gxcopnmym.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gifecpuvx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoyczvdy.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gtsosjwxm.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gusjerofx.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajfyayf.sHtML


<!-- 参考信息 -->