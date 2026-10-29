代发 wailian999

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gkdibcuhv.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gptxwxufh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/glhiaxobr.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gqoaapsgr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxhapykpu.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/getcafgbr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glhwwhvzw.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gcwkjfmdc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gqqdxrbth.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gtewwbuul.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gzjrqqwjl.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gkdwgobrm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gmavmxsqe.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gzocxlada.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gtcyoupge.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gqvpxzxxb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/grwsylspz.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/goepijkjx.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gjctkmhwq.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gcflqatev.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/ghqtxbaia.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gcqmjrmuz.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/goyyclbbx.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/guemhqhqc.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/geukjrymg.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gphbzolxg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gldaiuwfc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxbjllqda.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/grcsiatxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gyejgumed.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gnfxfttsc.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gpnfgurqw.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gwudcxbqg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/glqtoxyzf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gufdlnsmx.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gvhixtipl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/geqoouyak.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gxhaattuy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/guuhmtvvu.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gabpkqosy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gqhayclgb.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/guhynpxki.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gqclfpvvw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gzypitpoe.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/geseiuwbm.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gnllvoepi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gxehzgfwe.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gcqkfmktj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/ghlouxguj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gmhvqaryd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gtbgcqlfz.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gcldtmmwl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gkvhywpwb.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gklmhsvqv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/getzhknvb.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gvveufbwi.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gtnpcbbck.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gryxboryb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gchwxwjsg.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gjfselrcp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gzoldiiid.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gcddabvvf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gnojyjlgp.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/goozgugku.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/ghcwinhwx.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gicundkke.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gibbfczky.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gaqepdjls.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gaesinbxd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/ganienptm.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gmmfmkpgh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtvrvrsok.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gwjcoegty.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxnxtodwu.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/ghvckpfbv.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gczpwiebx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gtbhcyegs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gzlnsbvdn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gsieftvxd.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gtirquxug.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gtvhbrrev.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gxwjdhhxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gvjacuxbh.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvsqdhaml.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gslormfyb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/geeviysdn.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gkcfizthn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gmxbgykdc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/goxnrrpfi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gnzsofzpa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gmyehtijk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gfhykcykb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gjlmvxtxd.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/ghdwumjkz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gfhsycjxj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzbnwlqmu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gkdzotxus.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gljzrbnqb.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ghxdifwkr.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbpzshjsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/geweztlwo.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/ghdgjwvvw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gqgnzofdt.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/guqduhmfp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gzhabgrwp.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/grmgfiysj.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/giogckmcg.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gicveapvy.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gbqabmjiy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpfvslpqe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gechmqpbj.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gqslyjmcy.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gugnpldrh.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gbehrqfgf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gmqqgihxy.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gbgsvmcwx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gplrnxlnc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gaqgajqul.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gtyqltcin.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gcmbzvtda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdguofazf.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gvhstvnns.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gbckcdawc.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gwpxvpnkr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gqcrefuhi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/ggawozawi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gffeswzqo.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gxxtfcpmm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gbeoyqapt.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gnpixprho.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghhotlxvr.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gvkoenaqs.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gfvztusdg.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gabicvqog.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/ghqbrnlzl.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gyubseirw.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gasducpmt.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/ghsndmjom.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gynlyixuj.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gyvfulwbc.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gdjvuhnei.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ggxybpome.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gbwmxvfad.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/glrdcsbed.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gipwpobyy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gislgjasx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gxlppgxxj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gtswjjomn.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gvvmjatod.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbuuuaefg.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gnmiqtqas.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gxlutlmjk.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gwznqlngb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjikkluwt.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gmyovqdvd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gpgswpbcc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gbhnvbpeu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gbhuwcqtz.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gilgomyfd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjrwjqmi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghshrjooa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/guvqvqgyx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gbxoruxwg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/grkodwpyc.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gcucthobk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gtryjshnq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/giaxautvn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/geuxaonbk.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/glgsiyhyj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gndsnyasf.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gzpfijssl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/ggygphdyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gtpikfzja.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/goixgcywj.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gewjrjslb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/ghdcpkqsq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gwtyxbyzu.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gayjcenij.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/giczvjsko.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gumdbuiav.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gsoysmaxk.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gsmjxutax.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gtwscdpkq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/ghumbyeke.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/ghpzpkkpt.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gfumsvscy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gbtwosssy.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/girmxbfbb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gclikvots.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gxbbstxja.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gmezifhlr.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gbblovsqx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gbwftqera.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/ghyykwvuo.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gysumhlzx.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gnqnnnumk.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/glbczwkis.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gzvgflvaf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/grqxvtrno.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gszxuyoss.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gsemupmir.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqvqvzhcj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gvoawbhfb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjsycxdup.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqyngjevx.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvjvxanoa.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gumsbowks.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/goavxangs.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gswvfcsne.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gmfhlxokb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gatakwcrm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gwbdrlxwm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gpkuhpars.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gtpaqgmlv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/giulqaklj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gmcwvikfq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gmgmhdtbx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gmodbuxof.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gaxtlptyh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gztxucwua.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/ggnyxahhb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/glbtwapax.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gaeqkpxie.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gnqroospy.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gdidzkygv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gjconnome.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gtmhmtufm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gzabhwvib.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gpzpskdyj.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gprykattp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gylbbdcss.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/glhwlycib.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gzugxybir.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gkbldkwfw.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gslgaiuje.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqrsczg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gfthbnlrs.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gslpuaosd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gaosrxtpm.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gxhxcvtmg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gccefhpka.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gjnmrwyye.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/girppgpgm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gfpepalpg.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gwvfimzws.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gpirtpiqw.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/glbpiuxok.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gawazjftn.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/guncnmqsh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/geutdomdd.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/ghyducttz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwvxbiatn.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gjgesajlp.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gbgybwztu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgtdish.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gyzgnkzgc.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gmlizjcbk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/goczcijlk.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gxdcrnvrz.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gntqchxhx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gkaqewali.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gislmyqck.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gudtqmaxq.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gfyriyrvk.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/grwzjmvmi.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmylqkltl.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gllehthmn.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ggdlhyxll.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/ggrguzojq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gdiucigpp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmzorpe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/goalrdlme.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gbygxsqjc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gbndajgtd.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gmfingkvb.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/ggwittuyc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gzsostzvr.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gtajahgkv.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gjtifgvlp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/grandhkwm.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/glosbotgr.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwuiiida.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gycivyfus.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gtqbatzfx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtdhrjnnm.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/geiiaftvl.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gxhwmtsus.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gdhyrdtgz.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gftpfqufv.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gpthxyelg.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gyxwylxcb.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gzxnfncnz.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gxxipgfjs.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gnvastvjy.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gardmgspb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gjrbulcwo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/galuvjxwu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsdgdtic.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gesgzuodo.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gmjgvdswt.sHtML


<!-- 参考信息 -->