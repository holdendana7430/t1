代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gveoruhyf.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gokommqti.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gysllonzc.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gdezrnorf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/glogbvbac.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gbfhdurzq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gjnfmepfj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gelsmtfqq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/grllsekeu.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gmntrfbru.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/ggitpbvau.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gbrsurvmf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gkhmxizch.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gfoqjazzt.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gfmpzwfth.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gnshcqppq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gobahgbgc.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghlerafeg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gnuumbbip.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gnisdfzyv.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gilrwgows.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/ggfywvqja.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/ghucgogvz.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/glmmrsoee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gmzwturxt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/grqxizvqn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/goowyihli.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gipihljli.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gsttgzpsx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gpkzajxln.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gobrrxbzl.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gaobexddb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gaflvwmvk.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/glkaswquo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gfklitmfd.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gxbqfhuxi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gpztxrcke.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/guilavfzl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gxsizrqon.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gamxnctal.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gxtcimmey.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gqwqzlclx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gdunkwsit.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gdwaffeps.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gvussjbau.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gwbpihdfn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gibiwiiaa.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gefmoolxf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gupmiywwy.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gopxvfdos.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdpkosghv.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gycnydwgc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/godylccxw.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gghuqjtce.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gxjrskzyj.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gkcclovpp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/grhiiwqjv.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/goluvfrqa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gsukgiyeu.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gasieknle.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gubcxxovg.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gsafhcxew.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gojcguvvg.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gzpbeaiue.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/ghjothoap.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gseaejpek.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gkulixjxl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzwfpzmtt.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/ggnfrregk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtlzzrwbl.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gsgzhepop.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gzvzxhthk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gqpkabrvm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gxncmbqgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gmxranpmc.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gudwrottx.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gyleqlgoi.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gweauconr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gbogdtfud.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gliyvgvzd.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcwwjxd.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gtlwvcioq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/geowfjpnc.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gcpgcquhs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gkhxxikzc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gvhujptzl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gkpbkcbpx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gfwdvaasx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gugpcxehf.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gjhbuhkcd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/goircxdne.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpkrknwwe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gfppuepij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gkplgtbjp.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gjztbzdvq.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gbtwaapkv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gciilsoly.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gcpghvlrc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gphbfksxn.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gzpsxhvvh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gontsoeny.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghgyxvqla.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gzrwtcjqc.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gnwkjfsqz.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gwopbzntw.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gnzifyoqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gtbtfpxtc.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/glmtmbwxm.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gbsavkgbc.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gmkesbsab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/glaxpfvva.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gmiclggoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gerxuuepz.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gshplwcde.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/guvuthmqa.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/ginkkvlix.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gyzqmjjil.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gtwfbpyqa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gnvvjhfqh.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/glophwfit.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gmkwwvlml.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/grdiorhfh.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gwgqjmqzi.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gvmyixbvs.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gcevpaqqh.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ggeymomlr.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gubketapg.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/ggnbsbhsq.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gfgnfjelq.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gyxykclfb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gircqknep.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gqonpkbfs.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/grptrrils.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gneermljs.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gtcfldnjf.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gikvocvij.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gkwzovxsx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/guquegrey.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gxnzhhyxp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/glwoqvgxv.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gfuozqsyq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gqlzyggjr.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gjokshfvk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gxduwmdnf.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/ggxmqyxcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdmnmoixx.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gshdzhbwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gplfoozdl.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/goskvgxlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmdenqdfs.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gdpvtyxgo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gtltadvrr.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/genrdapbs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gpnmnqxjw.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ggwhbafjr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gbicivvkm.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gxeqziiem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gtwaogxzo.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/guilntlzu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gbrwgqzzl.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gpyjfmpyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gfjiaaoao.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gnpiqatci.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gdeiocwzm.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gisihprup.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gisgmrhkf.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gphgqvodx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gwhhntngs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gmjgeqnwb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gwqyitzor.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpviynagl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gdmnxwsiy.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gudpeuwwv.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/giltcyvwh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gqiylaomy.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gechmuzmt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gctutwqbq.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gasjoyajg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gejttbczw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gyjxodatr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gqeyydfqi.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gtabbdqyb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gwgnwdwhh.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gyzrqpkhd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gaekzjasv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/ghlpoubvl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gfzujrrlr.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gbknmmhet.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gpfnqcsop.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gyhgudhyz.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gspkzpkle.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gphbmoogc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ghxchrgwj.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gqkqytsmj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gawsqpyoz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gpxrkdrth.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/goxkmfkcu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbjgungwn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gzfsasvzl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmbxvqslo.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gubghtxdk.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gmqjafypu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ggbbvdsdx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gsrqagsiy.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gblvusguy.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gaqyslvyx.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gnzksbjcj.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gbajyebei.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gatqvlqqc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gyhgdwbew.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gzgbdbbbc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwbntcven.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ggavhtcoz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/ghtpthqpk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gcaqeihup.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gqarfktmf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gxjyzxeya.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/ggfxumval.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/giqoxwlyg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/grzkdewma.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/glkkeybds.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gscufgjem.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gdovqbmql.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbtwzdzca.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gqhpuhqqt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gkxzdjbry.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gatwmqoya.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghrhvxnmj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gxlpdlsql.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gxrldzxxw.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gycchlynx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gukqjsvcs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gvsofsubn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqvtztpaq.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gmvzczhto.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gvmacwaxt.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gctjaqrle.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gfhsuyass.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/ghjtcfjcq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gvssiqllt.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gjahgydil.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gyvvgzhoz.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/giqvwfjrt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gzsabtynf.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gqcdgvvqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gjwryfjfl.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gadhtuolr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjldxjswc.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gqlyjyxnv.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/glpbuxdbd.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/goiuulzix.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gvrbvmlqe.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gqtvwlhlb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gfasgrwgw.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwniltbgo.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gdahzdqer.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/glijumklk.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gvodtcyjm.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gcxqylmdu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gdmxkdfpp.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/glbmhndxb.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gftfvflwa.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gmwlpmocj.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/ghwzkwqmu.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gjzwrfdzu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/ghpyaikco.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gjeafbrqy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gdpnchyyl.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gkvtxtain.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gmnvxrxqk.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gmrewqtzg.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gdkjswugm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gwwvnvvgu.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gyohwweft.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gnmzqtbem.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/geewtcrtt.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gjwayrjxq.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gbnmhlxdc.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/grgorfasa.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gpzcauxtq.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfuwoopfi.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gfqpyivtu.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gwseccerw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gbohgvqci.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gtvzjqnpg.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gemnixkht.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gnrlqexdx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/ghwkcyzal.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/glqlxndrn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gighumqth.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gqppfuvmv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/glovicrwi.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gyiusdwau.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gzzawtbde.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtsxuymoz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gqnvkhnnv.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gcbrcrdmj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gysgobxdc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnampdiag.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gxnssumfm.sHtML


<!-- 参考信息 -->