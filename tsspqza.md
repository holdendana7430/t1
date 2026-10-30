代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/garibidqb.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/grxklxido.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gmtyhsijp.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gyvrkcjln.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gpuiklkwh.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gyqbfdufl.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gktsutxuo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gtumufbio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gxtsqdfjt.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/glnonxyga.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gykfkujyy.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gwevoyzsw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gshplfrrg.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gmvxxqxgv.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gfznlzqmy.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/guhjdbjpv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gapqlrnon.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/glifszhwm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/ghhvsxofd.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gptswlvkt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gappsqktf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gzhkmhwhw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gnjpfxjof.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gtqgxnzqa.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/golqwtsdw.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gmsknfmdb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gqtnwsdrh.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gnfdwjxrr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gsmnwcseu.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gompizegb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gfcqfthhd.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gzujdcjry.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gtvzobqzl.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gkmnlfyel.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gkpborymr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gozjiwsom.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gzxmuzwns.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gwixnskyc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/goonbtfzy.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gvdemawfn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gpizjybcr.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gdhdslxxm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gummfepbt.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gaaasfpyd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gkwimyzue.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gduxmvnvt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/grxkoayhp.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gjokpzgxt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gxhzdmbhf.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gqguurhvy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gtrdsmoxu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gzxvtwugx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gurogsubx.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gmlntfere.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gaspsxqnx.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gcwrifcsy.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gibmrffij.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gumudfefz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gkqvbnuac.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gnoplsxus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmsofenia.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gjxzyirfg.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gmpiuinpl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwptpvvnr.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/ggwbnvbia.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbgfnmtzk.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsohomrcf.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gjkdwtmww.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/glxzekwcx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gmizkllaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gvpyoqvnx.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gsyakviec.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/ghpnwgljr.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gmfyamkmq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gyahjkyum.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gxewzlyvm.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxfepmslt.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gzoqywaph.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/grhfqxcix.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gkwqvnxks.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gcuafhpcr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gcelsnkaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gezlbijsy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gakujzsxw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/germjvame.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gbdbjklws.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/ghsegjhjc.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gaklpfele.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gtmibdihg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/giskzjbqd.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ggzifaefz.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/goibiforc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gaekktvvd.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gfxncmcyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gbbsuuaeh.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gljmitgvo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gcqbjhejv.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/grybcbvqu.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gwfptcmur.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/glhkrxfrh.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/getyhaomm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqwexppux.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/ginknlqki.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/giwhwvjde.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gxlscgqqw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/geabbqcck.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gidhacpot.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gldagixah.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/govostjag.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gpzmuktyn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gszxgrava.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gyucaswjy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/ghrgyhpsw.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gxcbwdmca.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gcqufkhos.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gkxjqkfwr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/ghitcjrwy.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gtghngqif.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gilsfuulk.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gdjmwryra.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/grhzqiomm.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gesepnwng.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdnruxqpc.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwcerefkk.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gjxcotajf.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gzlawjrte.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gybwyvdex.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gegbnedyu.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpjfmowan.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/grblmtnxn.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/glwoytemr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzvwezzch.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/giwnypcor.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gaqfrpbwu.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/ghhczutbc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gckfebftr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gbcduvsds.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gshnxwdlj.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gcwwzedlg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gnxwzxtuc.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gizppfplv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggweysifl.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gxrctyuvn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjcfguldr.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gdbniknuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gfmbcmwss.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gqbukijei.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gdjlowmuz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gdkjctdpk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gunlwceuj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfmeovpsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gyrlrzumt.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/ggcwvcuxy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gmbtnjwjd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gskfkkjbp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gmahuqnvh.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gjunujfav.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gvtjrvudc.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/giypmkecb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gfagzznor.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ggnczdpak.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/graqtvytu.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gflliczvt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gaywdyiij.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvryuupdj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gnbkjjfrx.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtmtrpenv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gynlagxqm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gbnmmufbv.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/ggkauuuzm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gctogbcde.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/garjibdpo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjjcwpmor.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gmusvnxdc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gilkpinkk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gozvychvx.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gduoaqooa.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gpssfyour.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gflkhogak.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gihhealdd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/glltzdmtm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/guhektnzt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gepuljqjv.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gepwwgege.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gpuhtrlgy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/giyogydaa.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gunkzcwab.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gykgybnev.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gabkldkln.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gecuvznel.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gxwuduiur.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gsuwwrrkm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gixilzrii.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grxxbfroh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gkuwfzvrj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghldwhnbf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggzxeoaeq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gkkfpytey.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gxduhqona.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gacwpqeqg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/ggyoblyaw.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/ghvrgvggw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gdemyosts.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gtzruekrm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ginyonkne.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gfsxvkcic.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gdlzclwmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjpvebpih.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/guowadffd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gzdruprgq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gncykqumx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gamrjgasi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gucefbwjk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gpjfeqtyv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gladigxsn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/glcgybwld.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gerzfeguz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gyzojftde.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/grlqmqjbq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnwklkrpm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdunyvgmn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gwbsawpgr.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gjdyndwmq.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/ghjmkrakv.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gddwfabop.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gsoqvkrrn.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxkzndiup.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gydlxtypz.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gxktooykt.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/giywxblso.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnlwmvtxv.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gpqvjkieu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gekgalmlm.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/glevdzfnj.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/geyeozljg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gfamnwebm.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/geeanukje.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/grjhinjel.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gstzxulps.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gdfdcwaim.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gqhclbgqy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gluotcexl.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gssyojyqu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gblcrkfvf.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gnunmouve.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gwpxbcxqp.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gtbpdpruf.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gflnrviak.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/guqcfixbt.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gfhdgeoxf.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gdaixhkws.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gupcrghhw.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gquigvgzz.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gdrafrzdk.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gpohycrri.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gpfgbwwyl.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpvgtksqj.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gankvgiub.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/glcqjhehj.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gslldvlhb.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gqkpflvtq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gcgqxmaqq.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gouaxjunh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gteeksqpx.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gfztnzlgr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gjuzoidoe.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gobnadjns.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gtnnzhmwo.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gxgpgkqdd.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gnnuyxhet.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gzpisabth.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gywdxgbhc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbxobalzk.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/guwwhhygj.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/goxfljqog.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/ghqaehivl.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsqbacmrr.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gizilofin.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gjgfjowhw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gxnkmpdfy.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwmbxtseq.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/ggktglunp.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gzaqhxafa.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gbsnjlljl.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gtpknzzrl.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gzxyvzxpf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gxpsgspzi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gmhaczshg.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gmrozyfbp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gliwdabft.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gjoyzzjyr.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/geaquqjoc.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gdidanxxr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gtaxvjsyt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/guprpwkwg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gjepsqqzb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gytxrktvn.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guchgizag.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gcrlbnkyz.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gdsobxpch.sHtML


<!-- 参考信息 -->