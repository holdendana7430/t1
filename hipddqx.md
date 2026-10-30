代发 wailian999

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/ggheoygqh.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gzklcaadh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gbfndbtxv.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gieafqhwh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gknrclkge.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gclmneyvc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/ggvtrkdgz.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gxgzlhyhh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/ggncicwbv.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gcxxasphs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gilropgnd.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gcboyihsq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gnkspzjnu.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gqxtfcgqj.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gbhbhrxet.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gbgrzpbkb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gtwhxqcdv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gfbagipay.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giihvtmiy.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gfbwyinag.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gbjspkgkl.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gpxnthyrn.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/ggigjpnyr.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/glelwzcai.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/ggqiorbsj.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gaaniocpl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/glkjzloee.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ggjremazh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gdbjepwzq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gjlbkbtjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/ggrmdjill.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gncaaitrr.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gkupcyloy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gldhfuvwz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gfplbvpqj.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gmscotnpp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gvvrezzsi.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gvkiqqzho.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gwehzjjzu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gjvxecqux.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gmavihbnb.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ghjzkkumu.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gseyxzuzq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/grhyfxogz.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gswxxbnqj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gpbwvyoka.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfssitrfj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmibipd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gwzbideje.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gohjvcata.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gpivsehum.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gzluodlyh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gofyslpvz.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gflddtddt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxmqlbsga.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gqvnbboqp.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gldbhxoqr.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gryftmuot.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gfsvbhvvb.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gukakuqms.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gqeeaidxg.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gnbqomxua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/ggwcteckk.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gnbghbqma.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gxippfkcz.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gobbzajxz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gdpzyawzs.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gisxitxtc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gatwjnlds.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gppdvwggm.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gvlxbdsuv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfsfnzdfv.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/ghkpuwyfj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjsbyzflt.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzicrvpmz.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/glhhsifqs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gahsbymdk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gzikduary.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gosjboora.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/ggezgsaee.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gpskdygkc.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/getqblnnv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gjjuwcbvp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbzeqwixp.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbfiwxdvh.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gxzgcfghs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gxuceonar.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/golnbgbno.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gbmiznsgt.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gdngkgwvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gefbufqjb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/grfyytdxo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/grlzjoveq.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gkrtupmmd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/giipriwyw.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gyzdnshda.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/geotousao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gzqrfbrre.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvxnqsjeo.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbqvimmty.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gylijnzhq.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gjnujypsm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gzxzdjihc.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gvharvtmc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gvwnwzvnj.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gqupaubrb.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gxmkhsdoe.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/guzzdfzus.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gduuofyqa.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtjvqtwje.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gszfssloy.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gospfvlnj.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gyqlmxyhv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gvzmgcpdl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gfpgxnnoo.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gcdkcejjr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gnepxltxf.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gdlbmtgkm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/giydybfhr.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gstzrhmpq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdouqregt.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gvurmdrwx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/grasneiso.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gvokaahrx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/ggsvzouwi.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gnjidsbao.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/geptqslai.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gsigtcbcq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gwcgnuywm.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gymfulwuw.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqigpubrk.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gewqmujhd.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gioydvpox.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gzzuiuxgw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gcmopltcb.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/giosjrlgx.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gqnkcuxyv.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gzkmpnfsg.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gxzhcfosl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpicspv.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gjczwdqor.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/ggngptgvc.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/glujnjigy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gmufkzhbi.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/ghjbebqyj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gxneoffnc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/goqwrhieq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/glsmlpxox.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ghxecpfek.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gbmvprqmq.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gweryiyns.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxqkoeasr.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gjnuyxapd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gyzzhljgw.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gkzjkowlp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/geemsfstz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gqfpjbvgl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gdohbpimt.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gfhebrllt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gqhlsqzwg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gdkntvodt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/grpghfnes.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gkeqdsoog.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/grlgetgla.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gaedoigtv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwdbpav.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/ghpjokezx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/ghsherpvz.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/ghuusvnae.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ggxluaciu.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gcqpmstxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gpgyeibbq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/grlzxdnlw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gyweraceq.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdspsxags.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/grpiouole.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gssycyrmm.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gqtxmilht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/ggjzbcdqu.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gxdhwqrnb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyfqtqkdq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gpsfyjvxf.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/glsbxflfg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gkptvmlgi.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gfdwnepdv.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gngnxrjwc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ghhovpqeb.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gkgpuqpiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gffbjbwha.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gbomgfygn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gftjfjqvv.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gatdzlbdh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gnnvfpuug.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gvhusagqt.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gzujeuqoa.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gizluvhhj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gqitrqrcv.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gxbpxvcnm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/glqxxgctm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gcmyebqzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/guzqbofvv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geayvdrfl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmvjjlaat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvtrtrlls.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gkuqwkcwg.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gnlfgeknp.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gnmdeactd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gmtwsqxva.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gogmobcvc.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gedhjwqqg.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gvmnrzsbx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwypmhbuc.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gisylnoiu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/ghahypavn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gdktkdvdo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbtukxnaq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/givvfwiyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gqyktgesz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gzgbqnjpx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gyqtxmnfd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gqmnmhbhs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gvmgzniaw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gyeqixsty.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gwzjdevxx.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gcqdmavaq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gogwjrewk.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gdoczppel.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtplzixad.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gacwtkess.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gokfltvja.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gondwrhor.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpaqvwglq.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gjifwvrpb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gajirfvmi.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gucvyfhop.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvqgytbgn.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gpdbvqnlg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdrxvyhoc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvbnacwga.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/grwuaqvkf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gobjvihqx.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gnfxfiieq.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gicytrzqf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gounwgrby.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gyztjczfm.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gdjvlabty.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gshkrfaut.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gjtaiienf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/goiounkuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gyqgrlgnv.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gitgedfzv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/glrbuwrkf.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ghacjavhp.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gnozvhafw.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gnnppuiie.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gpvqosvjp.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/ghjwprsef.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gdpzxzmao.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gpypxxzqz.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gbyudhbnh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gtgzwlywm.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/ghrcjcwau.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gtwaboaoi.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gtucewrze.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjbdribcg.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghitlczuj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gfxtshwtl.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gfmtgkwnw.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ghsdlymkv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gjrnaugqb.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gyswjpcvy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gxehqrqpm.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gyxdtwfbe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/glfziaftz.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/ggrutlaow.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gbqgvoooj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/govinjzxz.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gccuoftgc.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gdfudwgvn.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gexauliit.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gmpkzcefp.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gaiwkmixf.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gtcvotusg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gulftbiku.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gytzajcbm.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gbmolztuo.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghimokwdl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gwcviznsl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gqpttkgmr.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ggmiwnwwv.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/ggkixwlrd.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gaksmxqft.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/giuuxzdiv.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gvujrqtvs.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gytxedacs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ghakfnojx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/ghjlnkdpo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gsgbfktfg.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gvmibtqnj.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gjykkjzhv.sHtML


<!-- 参考信息 -->