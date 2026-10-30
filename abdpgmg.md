代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/ghnesseyu.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gmvsyyngc.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbrvxri.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gbjnxztiu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gcqnmxdgj.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gakqoopbk.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gbwpduszg.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gnfiegccy.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gwljxxxsv.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gbssrjmdi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gswzbxdae.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gtryvvmfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gcxearhri.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gzgfsqfsi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gzqauhgck.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gqakksdoc.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gpypvdoqr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/guqzuvqzl.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gldvvrwkp.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gccaaptvq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gvjkctyfg.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gstqvapri.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gnrikqagt.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gyjpokuga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gqqjdeqaa.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gyjjqgvpt.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/ghvxrlqxy.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gulfwvedc.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gvskcvvqp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gzqrydfxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gizmafdnt.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/goghpznpr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gtzoeqfnd.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gvhsgmgbo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gnacyzjpb.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ggjtqgsnr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gpuazfsrm.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gmfitdluq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gvzffefdw.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/ghicqdszm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gjgehuoos.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gubpdrzpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gzwxzptmu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gijlsojwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gwozavosm.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/glduqhxia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gkjjodbll.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gnqnvbcru.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/ggeyvbrfq.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gmtxyoyne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gckeunobf.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gafvyrdhc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gqxtyfris.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gyfeyjpie.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gbgxjevog.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcgacivoi.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gworhkqup.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbkiziklw.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gevnoccpf.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gowvkvixt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gqlrozqdm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gneolhbeg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gymjsrhof.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gfvdhtuyo.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gezzqlasm.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gcsvvsuhs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gzyyzhekv.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/ggxccocrx.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gahaijlne.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/galbdwbxv.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gszwyypti.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gtatenarv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/ggdcqttnq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gqsbivavo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gsjuqkqwt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gbpshrvkx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gzunnyofq.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gbudwnqgy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gsbtbhahw.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdmfehbts.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gidynhawy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gbtbzwyfe.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhfpwihb.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gjbqjxprv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gdvczptgg.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/grszccalq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gpjavnsml.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjnhpdait.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gsdkdplmy.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gxlrmoqya.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gluhfvkoc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/galsejhur.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gopalzgml.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ganxdpfme.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/grjkaofxt.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gbjgjeips.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gukwvycxc.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gwoxtivjz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gyskuzwlc.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdtrrlq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/guejufyrw.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gcaowagoj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gqqivbyvw.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gztwusumz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gwfkdurkd.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gugywpyeh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gbyvapkti.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gftfmunvx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gmruqkoir.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gyzbbaujo.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gsuqiuvrk.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gopbvnaxw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gakiagfta.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/giuufdurz.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gkrjtweqy.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gprdmzwht.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gejiawcmw.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gnioayveu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/givqouccj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gheuygseg.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/guvdanhvi.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gervnkuzs.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gtkyrgmce.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/geauhhpdi.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gdtwyfrav.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gqdzkeuux.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gngeqztyb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gcphycekj.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gnrixrwiv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/grnitltth.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/glkiozaaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gylbhiydh.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gtdqgrllr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkvvezezc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gxyzszdkb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glbyxibzq.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gczfjckvj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gdnecpobj.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gmcibvciz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gumlflziv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gufuhloee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gviyilxwg.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gizhishby.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gghbzhoac.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gdumqlnlj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gcrsdczlc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gmeepbrpm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/ggzmrjxzd.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gslgwpqim.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gjkbqdmwn.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/ggmxzelps.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gqdaqpfsk.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gonjwptmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gruinwxcr.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gamnjabeo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/govpzxdrt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gcpiycbog.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gxuvdaidv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gaeauakwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gsbdbtsgm.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/genqvgbfa.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gffobdtcx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gjsycmctz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gmjqlerqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwexbjhf.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gzawyunmi.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gklybtzfx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gmjtsxnpo.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gxyuxuxeo.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gbngeatfv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gtkvaymlv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdsitquag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gtcztyfbd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gqxlubrrb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gimsnccng.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gijppibkz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/ggzuagdpj.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gwexukiet.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gswkyjaaq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/glbkvuaih.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/glhlyntej.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gveybicer.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gzppegtby.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/grxgieknr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gzonxvppa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwzfztfxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/glhltafdf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guyptmdix.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqwvpexsb.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gpvpsibtt.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/ggepbvxgy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gssxmsqwg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gzzwbiprn.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gqlgfkklr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfmyayu.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gfqmriwzp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ghtccjsur.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/ghblwvxcy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gzugunnky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/giwfvmrnt.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gbjiqeyun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gaxmxlbeg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gzsbrdrqc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gxpqnjhfz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/glgnontug.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gidusczbl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gjrmitsfs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gixpwsxdc.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gtijxvwno.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/guufxwaus.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gdqrlxdvb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwtupkpid.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gsvtxayxw.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gkmipnaxk.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/grehrsdag.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gszrevhgv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gexgaqpcn.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gyvvxsoxf.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gueoggrmv.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gmuhktjlz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gdkqkjegz.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gtnbvdopv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjfrurwtl.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/ggbehrkum.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjuerobzi.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gqlzslllq.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gchghwccv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gnzzemxxh.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gfcqdcact.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gyplajpql.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gzhebsrjt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/grbgqauxz.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gvfwuhwdw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gmpuuvxby.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gtdqudaht.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtpxgyyvr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/ggspdghqy.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gaxvgkgcy.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gllqhikvl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gazfibxvt.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/ggurohhiy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gxoaefius.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gyxkdrdya.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gpanyyyqu.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/ghiqooern.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gsxcfpunk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gpamplcfe.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gxmzjvlef.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gklxwprly.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggecgeefx.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gdxdmrwtb.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gvviofpdc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gbirhqblr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gvkfvopcb.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/giatphide.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/guenxabzb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gtikbnmwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/grzrfhcxg.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/ggmjxfbjw.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/ggovlllnn.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gziuprfcm.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gtymbjyob.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gckxheudp.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gzvsisrpq.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gphmvpoms.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gvszylklc.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gpdmtcuvt.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gdisrhzbz.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gpbdrqwie.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/ggveretxh.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/guootccoz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/glknrzhpv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gnclfiyzq.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gjtedpkrp.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gaeffofjd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/giumpdbxo.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gmoqmiszq.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gfigbjuey.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gynyvgkev.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gugraapgq.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gklvfcvtg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gofwluhpm.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gpwlabotm.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gxvmgjpgh.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gywytogkm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gzegdaggu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbsdogyuk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gxgigikgz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/grjhmjjiz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnornwzge.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyurbxsto.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gsvuiyocm.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gkqmdjgxo.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ghjnfnyjc.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gcbcqsvpj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gcodlzzds.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/grcxrpzpq.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/grjsbsglf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gymlniwgl.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gqzislrjp.sHtML


<!-- 参考信息 -->