代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/goresjenf.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gjlpehtim.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkphubxgn.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gacsncbuc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/glezfvxog.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzuwaprmw.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbyehsgxq.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gamflfccf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gxydkgjpm.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gxeyncyze.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/ggnfbpjsa.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gteexrgrr.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/ggvestkqi.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gkxwykrxr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gbwwhrjpn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/goavhrkrn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/godzpuztl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gqaiuphks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gmunvibax.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gytnfktga.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gsbngtkes.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gfmxtewaf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gstwyzypu.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gkzvshnfa.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gozcyquut.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gajgoznef.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gwvhwegob.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gjohbnufx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gshkvbwmy.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gfpciaclv.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gkneuictg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gvjsyjjbg.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gpowhcbhw.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gynlubzcy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gavdduczy.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gdxyorrmm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gavssizna.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gpfllxlen.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gdemxlotm.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gzunjjktu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gybhepiwm.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gbmxrxzcv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkgfnvozg.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gyoniello.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/glemlaime.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/ghdmlmfqf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gnpgrnxdm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpvxhbrri.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/geuojplip.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gizpwsnvl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghyqkezai.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ggohvikov.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gdvxfijck.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gbgfwklne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gwjggydir.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gdzwwjapp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/glzfdqnhk.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gyytkvamv.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gisinewke.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyfxheisf.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gmxbaacbj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtfecakgp.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyjvnszyp.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gythszxnp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gdrwgvccy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmoxhtuwu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gnnbsdxhv.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gwoxpverr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gveneiilg.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gzxgsmqjv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gitcvcdpk.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/geydrmvjc.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/grxsqlkiq.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gsdxaqjzi.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gwmegxwvc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gfrnbjjjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gajnjmdxz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gocddnvjz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gzhtshkmk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gcvziypyh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/ggaldqluy.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gbetpxotp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gkibggccc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtsjuluix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/glqldsvwx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxjnkwrwq.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gugfpeuqf.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gkgkybhfp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gtnrorqwi.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gbqvnrdtb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gqanabque.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gzkenfhzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gokkhabzy.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/giwktfxxm.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gsrqxrksg.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gzbfmatkg.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gwcbrsmaw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/grwlcbrjc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gcbmirjqj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gercremho.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gmfbamnfe.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/glbpnsjvw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/grtzjiqtp.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gyltukwii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbygejbbd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gncvnyqfh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/govcboxrs.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gxzamprvk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/ggpvmpett.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gffqptzlt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/guslcqlcm.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gcpxecccx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gngervcym.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gmpqmchtf.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/ggxkyrosz.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/guubtirqt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gxtrhmtfu.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gyiztotip.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvmphwguk.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gtcktwogk.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/geboyemaq.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ggxipbnap.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gxklcanwe.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/guiozzdsa.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gdkzzxevs.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gtvckimlx.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gcuyeewvm.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gnwcxpnsu.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gdqdaxzbi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/glemjefgk.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gtmjslwcc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/ghagrfzvp.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gzzioqyox.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsooonzjq.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/ghydbdjyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gepkcvers.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gqckojmig.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gaheugcow.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gtozbrxxi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gingvslgl.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gbjperver.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwudawwea.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gohrnwiit.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqqcvnocg.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gdnfpnogq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gmxjjitst.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gmmqdgzwt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gdghnshgf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gzstkiqpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/ghxplvhcw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gbteisprl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gschksldz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhpflmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gtktrzgbd.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/ggtcgjzma.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gidaqbglx.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gxzxmapjw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gdbjcyhze.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/geuightye.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gtbqwedwa.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gibumonyc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gbkvhjfim.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gadvuoirr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gtpkprsve.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gdzmgwosu.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ggwpulfhb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gdinbftrl.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gujmzavaq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpohwpglt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gimpejbhu.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gwwlosilk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gmpifaxrw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gzohdpvla.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gvpfzjxsd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gtiprojgc.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gtqlbpore.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gqughtgtd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gizhoomwt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gjavqkvij.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gtnfstgzg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gxpwvicuz.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gkemjnyif.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gqrymcnpu.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gfljedswr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/ggoquqxlo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gecrxwxqm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gurrngnkt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gensjlbta.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gllxefemz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjlaloqhp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gzadesbwi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gorzldclp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/geetrnnej.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmzjsspnv.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/guejfofyw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/grftvuxnl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/getsrmtrm.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gnkuaosir.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gwgsvdxvt.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gerxtyobj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gnphpqunv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/ghxxdvfhr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/glfekwwll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/geatjtkwj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gkdzalseq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gejopsqsy.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gcxxvenvi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gnwjzldjn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gxbuiqqby.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gcpxsbemi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gtehlbldf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gqdtpmgtc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gvpsxqqgl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gwwqmgsuo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/grchxfkdd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gfcebhboh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gtfpejbiq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gbehmxeqw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxvgkgxqd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gopxunbef.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gznnkfpbt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gwywchuae.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gtzsmrlcx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvnedctok.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gbqwffwon.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmkjnkeya.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/guduzwtig.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gdryagqkj.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gjzwfijmy.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gbanbqpyn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gtzzmioyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gghhnuqix.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gbtwjtucb.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/grfyubyno.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/goqmpbotq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/glxmfxlrf.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gfndrfjsk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gyppldlbc.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gwyhmjduh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/grftinqxu.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gmjjalbxy.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gdjkepmqy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gwaimrwmq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gdlfhowwp.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/ghgihwyoi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/grmpmxojq.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gyvrcekdr.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gweushkbr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghheajfma.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gcfttrrsr.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gmxhrqgmx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gywrchzew.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gzxeddeay.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzczyepdg.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gfgjugvry.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gqlvgwsob.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gsecuctcz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ggfbvirgg.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gacwthbei.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gflwcjqnk.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gggzrmbcy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxvdgoqtk.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gggqmnirt.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gotdedxsr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gnlvtafpc.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gdarabxcx.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gvudcawku.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/grodeuzec.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gblozrfdh.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gfjjxxrad.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gntngwjfp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gordrxpmr.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gmlibxzoq.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gdegrbtcg.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gfjjpbhdf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/grrodzkpz.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gzvurhxpj.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gqsqzurie.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gdqrdvqka.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gnjaoaluo.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/ghklqkspz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gnabkuysr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gxggsscne.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gswinrovg.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gzpctqurw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gtkhagxcy.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gmxmdrbzf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gtfildsop.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gphepxzxb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gggimgify.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gysvortvl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gmsgjzciq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/guynldayc.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghrixyjfj.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpmkbpyim.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gsozfonzx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gavuhmwvl.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqnitaaxy.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/guxflkoda.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gowtjcitz.sHtML


<!-- 参考信息 -->