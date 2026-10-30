代发 wailian999

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcqnvihg.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/ghxffgdcf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwokmshnp.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyygumwtp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwzjogy.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gkxghnitr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpghplmem.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxnebmmh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gescgwsur.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gygmssbmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwkvqvqi.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gkchgzbqd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gbnxdybrj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gxpwhjapy.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpevibay.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzppjppp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gjyubdglt.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzuvonbo.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchiirlmi.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/glnqxttev.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gffgkvskv.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybfngutv.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurefprqp.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnttxqj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrgwxepi.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqwakjpwg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gxqqxuwqr.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/goflmuetg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ggaykipph.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsfacjro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjfcpvzu.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gburqcapk.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjmurhsj.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gykdpgetc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyipycix.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gpkqsvdcq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmxihehn.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfahqdiwj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gfxzirnlv.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/grxgbeaif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfioykfk.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtasucasy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknumkdcv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gssnbmgmp.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gisjbsqun.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqnvosf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gejjjtbty.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbyisvbv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gkljuqrpu.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gxbyfwlzi.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gyazlfhlf.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvztrmhvv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gefzaqion.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfmwcyki.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoxvbehn.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtcarsuwk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbqvbbgr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/grellijtd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznbxgsla.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhdmurra.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeatuimo.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwjxtkiez.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkgavxek.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gcuhpzysh.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gdwculsaa.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/ghfidolfd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ganawelnv.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gxcmevrya.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gollsqjdq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gujdsrmtn.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/grvbzqtgg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyailbup.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gsimszwab.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnlfbsby.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guqhotxvi.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgugxkcx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gccdjluiv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gaupzuicd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxhwytumo.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmycvxkow.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvrtropa.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjcqqnej.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiwglxgw.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnocshbsd.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmszvxrn.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcvpsbsxt.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmgembyp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gemhtafuc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gsuruikdc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gkizqftre.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkslwhvt.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjsjggqh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqslebxog.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gifiojhxk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwxbveop.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gukqecpii.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gwhmavzfn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttelzlms.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmnwysry.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchwawsbw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gupqosmrh.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkrcppmu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gwkowbdrg.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/glvmjppgn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwjdhwqt.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwnyhbtcm.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/grxinprpn.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gmlsbylmn.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsznmjnl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuqkzjtd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlczrpjs.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gtuykpeow.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrjayxs.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gyjouszdp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmojcwsvz.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkzvcweg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/glhcpaggo.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gagjtmwfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzfqsba.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/giklmdbam.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gseijltde.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpawflrk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyftmnamo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxsvcnpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gvflzzdlr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqumyigm.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggggiekaj.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnivqjehr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdcqozl.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/geyumbhvz.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gahjhnxya.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlldxxge.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbgdlqvk.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcrxsjwd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/goztfhtgw.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gjdyecvvg.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gkdngarsx.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvulpit.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gtjvokhsv.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfzxjwdhj.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelzhodtu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnivnlstn.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdwnxmbsw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grrqnctlp.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gytxpyaeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjcobtvn.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gbpofvftu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glrkusitq.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxhydvij.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwmbpyxb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwsbshbw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjkqjchsx.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gyncoonli.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gywafimif.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giggjggcy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdnzmoew.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghohfmcoz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gkgwqjfir.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvurjqfhg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gburmpjcd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glyhwnmxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhqeyhxg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdkapjwr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gepkavijv.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmanummcp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmpztdbp.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvyvrnal.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geaozpujp.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gkepqtdjs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxsqjxgv.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzubuksns.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmfpscvpd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzjuwyfys.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcohjein.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmdilta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtylkbwup.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldqquang.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfonanbly.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgqmlqvu.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggswtugag.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/girsqfaah.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgghuibz.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gojwbxzwn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gynzfgwlt.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/glqxlqkek.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgnvaddz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwafepyt.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhruzaqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grqsraqot.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuipkroi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gtspzuqoc.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ghwwzgjbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxclzsyn.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbphjxvix.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gfsovtkkv.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutajdqiu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbevhru.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gfewzouiz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvzwokxh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfutidnnf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxuearhbm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggwqexdry.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukmzhbvh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gswaxalsi.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/garfltjeh.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grgtwchfr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcjlbdkx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gciibnlna.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgrdiatu.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gkirpsspt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxjybgxk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdenxqxqv.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gwyscnasg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gkqomcthk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/ggtcyckuf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gprwvdknd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvqflzgd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmjbcknu.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gvhcazrlm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gjwrbdajb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gandizwhl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzbydtnr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gavfozhvz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gldpaesmy.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gjhwpeybz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gcgirzlhf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gzszeapqp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunycsfkh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghxpldmnt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gykjnboix.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gulivapuu.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvxndeod.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gnicysjyg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthdszycv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqglduqng.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gosthmkfd.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzmogxfcf.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmfjpfl.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmzkryj.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsnrpvzg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeffjijo.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvklkrfrk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/goudyqewi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvislycy.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkaqfijx.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/ggjysxnus.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhvgrkji.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqhcifphq.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdqcknrc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqtters.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gjfckvnna.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gejuwohsz.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbvkwwyz.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggizjueiq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnkvefob.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/glltnmsws.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduyxtxrr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwesinhf.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdqafbyo.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gfiijvsxj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gdssgtago.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gmsfgtvmx.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyjekudt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuareucu.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guebhlpvf.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzzlbfw.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gidundksn.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gyclvhaik.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvkazrbs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhpdbxnz.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/ghjdhntyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoptfxty.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqohpoch.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbckijdcg.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghzmomjfz.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gqtgjygzp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gglcxqtnu.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/ggmjiknnl.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkqrixwe.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfenwwzj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gazavtrhs.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprietcmy.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrnwtpnh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gglzslqlo.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gspatmcbu.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gayanwdza.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/guicxjjak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gssaoyfop.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphykffxb.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gjnuvzsve.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gothlrkcy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/giyghbyaa.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoljegte.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guufufmzo.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gscqcrtcp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhnrtrtw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gogysemwo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcwomhic.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/goqzncesb.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gpuiupvmp.sHtML


<!-- 参考信息 -->