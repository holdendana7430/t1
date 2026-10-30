代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gklowcmap.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdeyeuly.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwmwyirfc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gjvzlypby.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/guxbwtyuu.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhjfolnj.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfdmjttl.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofzvpalc.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/grxjyydke.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncvqwfir.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gbrvucmwc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupioaynn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gaewnosag.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaqdokxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvuutuqs.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gcpchkxig.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gblfxcxbs.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrzpsxwz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grztwouqd.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghofndwlk.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhsazpjd.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gthxbkrxg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrzkdrdx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpktzevd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpnhgdjl.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsqvmttr.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gimoezkmk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gautfshbj.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gcxktrqyf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixblcvlw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdxqfkwys.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmkodrie.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqemgiq.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gmblmnzau.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/ghuyumoat.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvlqfrwoq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmuoeltm.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gggnkuhtv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/getkzqjch.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdmzyikaj.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gzgeyfmey.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gkdebabju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjtxbbs.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeciqxcx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuzudjbt.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gslwonmbx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvrvisng.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/govdrndiw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/galrbyfiw.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gilhpjxrn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfwnrlutg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmohjzaz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gofbgnbyh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gxqnfuxaw.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/glplbdfrr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gaeaisrvo.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/getmwcpjw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxdmwzht.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giesecmcl.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqeieljl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbnvnxiig.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopvvdvqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkvnbril.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gxiawedyd.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gexzibqpx.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcibioof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gpuqddqsa.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviflbmrg.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/goilddkds.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlexebvu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/grqtruudj.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gptfpgcpm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gyslldsug.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gnyvigoid.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ggbefuvuy.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gaemkamlv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gkmgitgvk.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbzdwwzp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkltmgusx.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvupprfw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/godexfess.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxonbmvfx.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffxbekff.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkygrpjb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ggdsukdxi.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gyontwjou.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gixiggapg.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/guvlouklt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpprhzahr.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxahxlb.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gweepvvur.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ghozzjmfy.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtnetlbni.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkpatbgp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzgjncep.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjizpunwr.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoyxefrz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvomufctk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmphdtzq.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/ganocltty.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvdwkup.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxisdhja.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyebeucz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnuxrrkl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gselryejf.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gvmpnagbh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guonionsb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhixsblm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gepvatytl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmlpbbas.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gluonkgvv.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gpphdhwlb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxnfchh.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfksipdcf.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/geglpilbs.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gldxvbleq.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnmcejrwn.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdzatvcpm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmfonozd.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gpjsvzryg.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggabxarew.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwpgkmdh.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gnjggylcs.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gohzerwyx.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmzjiqi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzlqxgncs.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwaekub.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlsyyoi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpurzcqv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubwpjzsm.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gcdfihyip.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbepignzm.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiwyzkjm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxofuluzz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoercxue.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbukkjqaf.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gujkccgta.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaimjtda.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxxkdxbuy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gznibchwv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmysxkezl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqgnqhgc.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbdfprka.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/grdoymlwu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcssncvwg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gexqzarto.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmoswgqod.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/ghphhuckv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcykedfwa.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeirrvpc.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gezrjqxai.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gplnedkgq.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpizsxlir.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwbkkdni.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/ghwysgiip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfnpekpo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwsgcfyzl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrhmgkgh.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/galxcfjxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjytibqnr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gjzwntczi.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhwfieq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpspdvwbf.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gidfvvouz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumsyumdt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gszimqlvm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcakffupg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gnwlruotx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/grvwzogus.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gwdzvflhx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxglerrno.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gzegxsfgx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gizrmdvdn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gncejdzvy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnvtytmm.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/givvielzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyapikjq.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gcouctmqd.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gtxfdivdy.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gbwdsnodm.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/giaqforkc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacywcccj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gfgwzfqjx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemltedc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gursvvsrl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdpgaier.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gydcogzgv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmyssqbte.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzxovbsdg.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/golcdbfpf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyulgfod.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkrjmqpw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gpewtoivf.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gtekfyieq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gapcrdaax.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gatsyhaon.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcwrnvofn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfjgzyp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdwvvgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaahtvcba.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjjyusxt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpbjmrgz.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxvqnabby.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gozqszkld.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/giqxvumhj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gnjezwcxh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gklnmtzqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gurrjhuyu.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gstkqiqwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssvzisnb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/grnrvhepl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/givxffsek.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gupxivzgt.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmxxlpzq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppokhmcg.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbkyhiaj.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyfxupie.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhxbokw.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guurocayz.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrdzxsue.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gskrhbbgb.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gofpodlnc.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkwgahcaf.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gpexohyvk.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gltmotlfo.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmrqddhy.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozcadkhy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gpadzaoew.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrwzgcpf.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxgstzvrg.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gjowgoktg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gombdclki.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozphauvv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyabncvq.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaktfdma.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdbsiaaw.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gztwshmta.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gyctofgmv.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gurkqlkco.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gobwmevyv.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/ghsugoaxx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrfmygka.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmvnaewjk.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/geafjuxrc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glasipbuy.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzqezlci.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gcwteudkv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpobjtbmv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrqdlafu.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gypixunys.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzqzesdj.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gkvtpntas.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gjjqrewsr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gakzestty.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/giuprdapq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gtwytgbub.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gaczlxwkb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdibkchgi.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfnamkfai.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxmtgbh.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhhckjji.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gugwlhcol.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gebgwkaqq.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gipsiwmtl.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxxdczufm.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gphupgbrv.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/guknatwyx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gjolvsjoc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofmecsxv.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzpofzni.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfbhcvir.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncjymjfg.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgtkyjvf.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpppzvlx.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsntbteof.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gknevyciw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbatvdkpj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gycazkseq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gskafifpn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvkbwkmnj.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gnhmsleuh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdedburog.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goocvgoll.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/grzcmffhn.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghycsuqzl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddmezioc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsrqtitb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylrsjgqa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcuzvtsyn.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqbaiivgx.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhzwczm.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grmpyyxvt.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gosdlweul.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gdpejidhr.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdcafmxg.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/giuidjfnx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gztfmsqnf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfeczih.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggphsgtcz.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/ggicucgwa.sHtML


<!-- 参考信息 -->