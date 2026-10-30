代发 wailian999

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdlxreda.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gprogdmov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gsdkxszxh.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirlbgbd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdumjlk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggoekqbbg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctaboiw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfktxcrcg.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gpudtbgaa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gulbwaogq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gpozvcgtl.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfihytdup.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbnjgavl.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gazaixwcq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsmxjgzu.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwqlssqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpmksmuy.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gprojgslx.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkfcywvi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeoucrak.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnxiyyw.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gdnrlebvf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gelottibl.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwvkytqz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gaftqpvtu.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwynvhqob.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gottrtfft.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gueaxhacv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoctjsdi.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gkmzeiayz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajyeyxft.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/golqxqgdg.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gndshuoxx.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gjrlbafng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grazwwasx.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gaumcxnmz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgwveqaf.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtawuiyck.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxchgtrwc.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gexrxfzej.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gcessjzwr.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gftwdkpff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gujwibnab.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gggmsfnnr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gybwwnpdm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwlhxxed.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpagdivo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaypihdw.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gsgyuodly.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoavppbn.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkxirmlp.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gezoiqxdy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvhrgvja.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmoimyus.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/glesjhtap.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokrwvdih.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjthzrju.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/glqrjaqpy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohijrkra.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvjfbpxx.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbvpmkav.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gefykkscf.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gfztwgylg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyesmammu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrerkgma.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gthtsppfh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplwvrbfq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gdttnuvbw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gofycswvd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gvwfdxdjw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfrsoalt.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvrgshnq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwfdmydt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsaznuew.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbaoujpf.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gangzhczj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gkimdypcb.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqxfblyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/grgviwxnj.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjcfgovl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gufwfajke.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnugpzgj.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gaepjgoxe.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekgteip.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlmctwfr.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhaivill.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjigtwqxa.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giixvzdyt.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtmdvgib.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjrrchn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/glsqlkilm.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gduloxjni.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwwzduq.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlkdabjs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqsvdfu.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gnocfkyuq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gekgpsalq.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/goatdxrea.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gckylsycd.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gthdwvdvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gruennrog.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gjhvywfnl.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gxtgotjbi.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxhpxgmg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfgrbfvxh.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gafspokng.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpbapmvik.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggoohgdhu.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcevuwww.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guygwqyig.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjjbevsf.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsxkwvrq.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gurhhncwx.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscxixoje.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/giemyshac.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfiqrbsop.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gyqkfrdmg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gszsnqdoe.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guylgwbxq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjkckaam.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gcfftasbp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gccxlqixg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkqqepni.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/goacnoytk.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gcfyiqyzv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfstjpdjy.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlgakgox.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxageqofd.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gkgdpawwt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghinqepio.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gairbsctb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gkrxzdhph.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gswqkyugq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwftvhqii.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhhmczk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glojrolmd.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gejwfzhvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpqogjxc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuhgqlbj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gzgaenhoc.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gvzutmmoq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gmmujfhno.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiohasgl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlmbytfo.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghamszeor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefeyvvvo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccgjsmoq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbvgccjo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyjumdnpz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdctcqcty.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvldgxvie.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gatwplhcq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeeckwdl.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gksnumyln.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyzwemer.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gaiqwpgru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggotvxjxa.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttypthhd.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/ggxafiwnm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gmbvwfrbn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfcujiuv.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxyxrqlh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxewaslz.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gumxzklmc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjznykdzg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnezzydio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcviorgw.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gsxdvymhq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gydwzhgss.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgwcehc.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxyvgnf.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gufnmwbcm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzqfkchz.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtfujiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gfrfvhrjm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gurdudzid.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxdzhehz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbvlxle.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gargwwctq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gweczulub.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxwqonu.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gtlmcmnhn.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtcefsowm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gxgphohgn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gqnbjstfb.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzmbxlzz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrcmbbpk.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gcydrxxmx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbhesommw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gputprclt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gigyzdzcp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsaweqclv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuruoenx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/glczydhlu.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gpgvyflim.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gjoowzvso.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/grjzimbfb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqqntwfs.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnwlmuzk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiucywvr.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gmsxicnfz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgzqifvi.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzqfcitl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkngwjrex.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/guustotlk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgndixwg.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbyvbafyl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehzdgsjl.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcfylggr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gauwhcats.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gounpsmje.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzdaujqeq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gehyklvfj.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gehazsnyl.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gawvfckqz.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnsdxugt.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gbqqlmvhd.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvemwvyjp.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/glkdblivi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gmyakhbww.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdceezytk.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfkuzwro.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyjoozsk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqtbbjrt.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/genxpcaaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gmsqmdjih.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwuhhadm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzabjpkbv.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gebfqbkik.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpoxxnqe.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmgaryrn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfpoxbs.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gfeaywfjl.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycmzrtgm.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxaaibvz.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/geboszrzl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjbdxjz.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/giktkeycr.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gviydbphv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gquaqyqwe.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezbgiebq.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxysrtfyk.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzylkcded.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqeilhsq.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/goahcadpl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwfdvvyn.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnnzwcvs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxbradsx.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gawrrviuz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsvqotmx.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjguhfldf.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gqmnqezxg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxzndghj.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkrgunpo.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqgggco.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/golviincv.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gznfytetr.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gledmvtxv.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpdbyjmp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmikyusvk.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grgindaqn.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gclcrphrb.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjmsdzlj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gwfhxtlkc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgjxiznk.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gvjjiwvlv.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxrxgvwcz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxylxzoc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvepzua.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdzqggifn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbddxiuuo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjigxuoqe.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gitrrplsk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvmsebv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/graoektfr.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gzdsbfmdg.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gafrfxeig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrzrwkgg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gupxfbini.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gxonvdqay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhkylqge.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxwyeohdt.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqfunmnlg.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvsxolwv.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gciyigknm.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpcrfzgu.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrmqpjsr.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gnslpeqlg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdpbmotkp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkeakwdu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxbfsqhf.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gnndkdize.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwahafqqa.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gljwznbpw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gwetilduz.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gpaaigilr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/grvkmqubg.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/grccslhas.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnycnrgsq.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/grqrxzazb.sHtML


<!-- 参考信息 -->