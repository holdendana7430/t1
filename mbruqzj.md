代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gpwytjyub.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgwldxxr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grwznndzb.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwjwtsmn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/giwabcnkd.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/glbwezvyu.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndirzdvm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssinncbr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/guycjczsi.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyfmdvxuq.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwigyzbbi.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gyziptbpj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ggylevltg.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsofzdes.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuhmfogf.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gkonzhiaa.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gpeqvlrpg.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwnxmsnk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcolsar.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gngiwwjkh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gsvukcuwz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gyfbuhsgf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/grnnfdsws.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gdcgpsaaj.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gcabmrtvv.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghhmpggjl.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gozhdpmnd.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgffcbud.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxmrnkxm.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gsglneazq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhlwlajh.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtxjrqokm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gbneraocu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggueyugyy.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvomxrylo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gdtcfiltz.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbwktgkj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamkkdxyt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfgfliua.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gebiwxsuu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjpczek.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/giiweblje.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkcvylnz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplaedbiv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkyydbjk.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gddwcuzqy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/glabafzyk.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypwwmvmk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gumzikjti.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/grtlqysct.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlzjetvj.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcefbiuho.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqljeckom.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqsmgzrz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjatwyio.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gfubcmdcs.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmjeypoc.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gabrhzdum.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjnspqm.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslkwpkg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfnvzyhq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiegtlea.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnaznhmn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grvhoioap.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmywbhupd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkaadnfek.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxdxijw.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gjmtksnrm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnoswjdnn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmhijvfl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/giqfwrlha.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjcftyfn.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/goaqowbal.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gaurfrbhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/genimdbmi.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmepqpfv.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbfminia.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgnueipt.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzqjxfcc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gslakoxsn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/goenmuknt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gjfsjhuvw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvptptftj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gegmnbvrj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gqdokptnd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gjzzjshjy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gujwsyzzb.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjemyisng.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvyalcvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/griwbzztd.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtbptrkx.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoawlrmb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpeqiadwl.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxnegapq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfcdgxfj.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gfqbxbpfv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnszjxzc.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjqmxkptt.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwqysahnp.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcavkipn.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/giouhmijx.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwxpncsrg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxknwgwr.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeandnof.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/ghsonepjp.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gktcjxvsw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudfcuuvm.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwqixfkq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/glxztqcjl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grvuipacs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdajkpqj.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaociqbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/ggdurotyh.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/grzmufhff.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gbjwzbbcb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gseqsnbnn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhvjftyh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gntopjyzi.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/glpsdozhu.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gtwslrbed.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwphpysm.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkskihklp.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbfkbjpy.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgbnotau.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwchkgfse.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gguiszxmz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ghpelodoa.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gsnbtysho.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gkwgsiunj.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbljwfehr.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpdeozxd.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpirtdoox.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwfzrucyl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopncsxsy.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggxgbicky.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/grkmrwgdu.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrqafllr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdftpppli.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gczbqwymz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gocogwwiw.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gstsduspf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbspodcxa.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbanzwyx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmavrclb.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gfzevvlhq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcnrxgov.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsqqvhba.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/goposaetq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gztaxctao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgyyfzxf.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gimbvyaab.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gohmrtpyg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdandylw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhuuxvnn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmarhloys.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gvzrohpzu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerayxybw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gqpstvkra.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjxwhdj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuxieaq.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgbwdceb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicjpohtc.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gydfpntyl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghysogzeg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gscjfyxzi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gohdodcoq.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjlydcxcm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhqkohj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggajiktym.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghmszbxss.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gbbvdsvte.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwyipdyu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gvanxkuas.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghzwqnruk.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbvdbqqu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gqccnepxr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmbexhqpf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoacnnnx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gsnofgass.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfwtucayw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gftavijra.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnqfbtln.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghidaitqd.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gerqxpxuk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdcsbrmjo.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnaubaqq.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gitqwxinq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajsfqicx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjpfsdve.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsxkwzae.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gjxscymou.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnchlvmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnzdapr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gutarxhhd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gauwnnoyb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbkiftvw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gexykcobr.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/geoofkkgr.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkcrkszdh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gsauxhefc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gwgzdgojf.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhuetuke.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeqcoqyl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjrgohbj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gywjgnydm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkksdzwe.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gjurbttgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzkefkmy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlzdhflr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcabfais.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gqseubodw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviynozli.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gifmrshul.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvbduxm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmctiewuj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrtgmqui.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntjglduv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbstnrfip.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gcxjwawdq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grsyyjffs.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gfceowdwl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoqnthyu.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkiiqqcdm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnvigwnk.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gtsoblmjd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gllhwllws.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gylhziiyy.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkcnymhn.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbahhax.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmggmlpsv.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtmeckfts.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkvkwjga.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/givsohaka.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmtkxuui.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gtldxxpvs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskewdrrf.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvibtxesm.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzaaaheoy.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxviohvg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhjfozcf.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqamocr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gkbptccqv.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfwirjka.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gumbpfogd.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gjglpyglo.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqciqjwc.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gzhxbdkol.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiqqgjud.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grifosrzc.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grrlqvxru.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gxzofgpqd.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrisznvm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gysdsryxs.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghenuyms.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhdmgljc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqqvfoyx.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gidxwqwqt.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guagitcmj.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grznqqmsa.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gkqjfptiu.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/grndlxivb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidinzoqv.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkousvdsd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/ggmonzmxi.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gukitpnue.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gexdinzpw.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxsluwba.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrgqfgvq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gcuqvthvy.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhcmuoqn.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhjnsrvt.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gaprztajx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjjaegw.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gillutvss.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gspllzilm.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/geqkxfoyy.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvmdlgy.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjvszuxb.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/glqnhdqnk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gwkwdqkmd.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gancdbhsf.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gouqnqypm.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdjshwkl.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwavrcdwh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbohajdv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gscawlezg.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/glghcmuje.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwmudrhm.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gnrcgdvau.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfggaatwm.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gljgcajhk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdkrmps.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdkmroctj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/geppytpcr.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkulsaeys.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhvmowqv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjcpvnwv.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqxvmvubl.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvcalywm.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqdhldcjf.sHtML


<!-- 参考信息 -->