代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gpsihknwf.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gpepwqtud.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gdllaqnaf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gjpignlvu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gyouirslu.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxqdmiktw.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/ghgsgwqsb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gydkxftrj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gqlcpozxs.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/glqzeoqoi.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gbugwwllo.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gmrwvtwaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gqwoeehqw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gevcfzocz.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gkfqrzxhr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/glfdbbwrw.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gvmkowlcs.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gleaekiyc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gkldqyvtp.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gkmepqzrz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gjplqpjmo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gmlzkstpg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gubzmckip.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gtkfbetvi.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gjfywyeqe.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gwtlgavjf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gexmyllgt.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gxnlcdfzh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/ghlcizdrh.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ghsqvbpgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gkecdrbbj.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gkpeomeei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gebnhgnpn.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gnnducrao.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gkoyltagz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gejgsdtta.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gqycnlaaq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gulurndiv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gxucjyara.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gxmvekrea.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/glspyavbq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/ghbsognfr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gkgrvujtv.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/geybmepen.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/glgtqpfej.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gymdtbubz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gwpuzdelm.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gslemgaek.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/ghyefhqma.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gqdffmwdg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/grftuubwk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gblywwbep.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gstchmbym.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gzqkvhfgd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gwrrcjzcg.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/grxzjstna.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/glrcgmgwt.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gsfaddvjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ghosfvtgq.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gkgnxjazb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/ghdixmuks.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxrpmdezd.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gakmmkxyb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghtabmzbs.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gorggkncc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvjrrqrhz.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxadxxhlk.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gqcmfcimk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gzewluegb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gpkxqitdk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/glhwmnfch.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/ggsxlvbwv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gzgjzbdst.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gbmzzbbve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gkgzbnlzc.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gvssjpccl.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnlcibqao.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gwpjuelwf.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/greuddgsi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gwrioteaa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gzprwppbs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gcsnkuwrh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gzmpzzyti.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gdsqrxwyp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gdvtjqepp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gnudragnj.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/grtbqhuwj.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/guozgtwbn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gulqwykkw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gyozuhwrt.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gshsycdjq.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/grtrrdsas.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gakqcurmu.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gyvnvmywt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gnxvcdsyi.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gqafhhmmw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gyzojfhlv.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gcqoepbio.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gamvkjeah.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gsnqmhzzc.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gdcsrmzbz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtzspmeuo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gunhojiml.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gwcfkbecc.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/glxsdacih.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gruzjdvrj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghsbkzugn.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gqkckudeh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gnupdivnc.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/grjycqyze.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gsckytyqd.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/grvnutvse.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcfzgjpzl.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gcyrqaisj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gzynnxfjq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/ghcsrngqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gsmrqvkcn.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gyfbdyfhp.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gidnlkdpg.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gwzofzdto.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwxzkimpk.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gpxskynqg.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ggdyatxzk.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/ginszyqfi.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gxouwajod.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gubcjduzv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gvethikrl.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/ghuivuekc.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gyiqearst.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gepilxczx.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gbdtqdaat.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gortrpdps.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gtwcvoynd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gnuedimsu.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gzulevrqi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gmbiyjryp.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/glhvkakbr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gadrwfbse.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/giivhlzdw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gvmlzidmj.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/grlemnhef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjzokwdty.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gsdywthbb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnfwncoeu.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gbmihrbdb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gqvrbgsjf.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gdfpquzaq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gliowtmic.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gnxxwvrkx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gtorytkyh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gvilsqfxo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gzspaquqw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gobkhusyw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/ggqsnfkdk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gdygujcuw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gydfjtrpv.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gytkpltrn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gvsnikxuc.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gsfhlgxye.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gfbysvwvp.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gzoxterzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gsjbqksac.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gtyygwxyx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gtjivqkpg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gqkijsauz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/glwszhmts.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqjqrfivm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/ggkwqjhss.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gcipkehba.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gjfykahzg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/glgumwjnx.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gvrfecznn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gazdejnrs.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gifyjolzo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gjenpruat.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gcbdibpau.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/guaohtrba.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gzjctnwnw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gdbarvdnl.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gzhjtafzz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gcxoazelh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gtmvzxopr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gzegyfkeb.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gwemhhwbr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/grffyimdo.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gmwuvmnhe.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gncirvpbb.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gemquomtw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ggsdvqcnn.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gjnriktbz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ghrsafyaz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gknholvfl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gbffkajiw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmpmwvwtp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gbqfxchzk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gojdwhygh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghissojuk.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbxjlqtyn.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/ggvumpxih.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gorajnotn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gkvvzdobd.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gvzfygfid.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gzqqzogud.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gjodvhowe.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/glexxttol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gnyeqllob.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gzytksjuw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/giseqrhsf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gyqbjztzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gfabjmzeh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gmkrilojt.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gzdyepxwn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/goxexdzji.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gqpeebkuj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ggklpbxco.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/goqkbnbvc.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gljuwledj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gtgwtbrbt.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gtobtwnfu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ganjhtmhl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gdgahsokw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gmqbzigtf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gdsxonboe.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gpulnsjfh.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/ghhhskspx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gpizjurae.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gddlvuczl.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdgjcyhek.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gexgmjuvc.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/godhlsxbs.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gflkxodaz.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gwyjzuzrf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gplzupdhd.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gtqjhcrno.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/godzvplgx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gulgsteuw.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/giquyvizf.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gyiwdoajz.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gazyvlwls.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gbjhgrobo.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gpmtwmskl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gvymhluhl.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gfyhkvcxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gnoqatzmf.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gbqtfrfqk.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gfmbcicrz.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/glsmacpau.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gxniumetp.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gvrrsmflc.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/geanclqad.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gahwncmce.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/geqekzhfs.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gxqmxgfmp.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/ghznddyzv.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gvdfsdtrz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/ghujfurpq.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gjtmzdfds.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/guxnmjcvc.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gqotthcub.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gulvqykzn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gfyoksabf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gpvoncimw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gnjfdnlpt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/goutedbac.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gsugjferg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/grkgveujb.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gfzjpqcdj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gwiocxpjb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gjebycqhq.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gdxbfdimm.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gqjhjtqec.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/grrqceugh.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gisxiqwlm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gaukqblxm.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gymoeucbo.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gqicjmiva.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfgiukszp.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/ggfzxusmk.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gslqhfgoe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gpaylonmr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gfuqrmzhl.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gyublzoqj.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/glikfkbmp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gcfldarwt.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gxpcadueh.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gigquxvkb.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gzdwvyynm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gkznynbwa.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gtqxbjcol.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gswqyargd.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gkmzouixm.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gwvbecuxb.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gqwirizbz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/goydnsrqx.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzaamykvo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gvhfquxab.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/guulhbmcs.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdacrpuka.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/geiuamwzv.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gipnsecco.sHtML


<!-- 参考信息 -->