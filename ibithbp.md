代发 wailian999

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gxbhcbfkr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/guuinjpvl.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gsxlosras.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gggpzzayc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gtctsqgpx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gswaavctb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gmaepsvop.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gofzldeeb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gkpegeuhw.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gptmecwjv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gfrfwkuls.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/guhtcptrv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/grpmucagt.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/goovfboqi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gufzwijuq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gvsbzoanh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gbkkailfq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gsbfigujh.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gvflcxwua.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gibevfajc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gmebrszqn.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gzvzgfzoy.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gcjuctnis.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gpvjndgfw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gaphmvhie.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gjpzldwiz.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glqokikjj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gfqiaxjur.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gcoipkoxy.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gngomxzog.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gxkxhisux.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gpomeypcr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gayywttin.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/grbiizlbf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gtishnqdk.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/glhgcbzvy.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gxhipickc.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/glrrcpxvj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gmyeocjbq.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gahoxrozw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gkcgdprsu.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/guikjrply.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/giuiriaco.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gwappsfxi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gqdniorew.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gnexcizzx.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gbmjzbjek.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gtivqkwbn.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gwjbbwbup.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gtvfzygmx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqqftzcpj.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gvjiedthj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/ggiumcyir.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gdoqlphkm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/glhsuokfh.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gowqbqxuk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gewpdhtpu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gsdmtogsx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gzxlcvgrc.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gvniranqn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/glpnlrmcj.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gmkbdvmmc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/geurzhkbi.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ghhmnevvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gsnusjdim.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gkajxrpkw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjajtynkc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/grdakkefj.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gjuilcaac.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gtsfyqfxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gnkxxfgqp.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/giieytjkh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gbjeqiohy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gpjqxqyhd.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gihvznaud.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnxarhehd.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gnjsqimnx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpnpbvbjz.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqciudlvm.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gdkihtzyl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gqtqnrxxw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gytimqcsm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gjmtlwmml.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gkpqtvuzc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/grcycfufc.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gbjynyizr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzyvrglat.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gxkmabuxy.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gzxheqzud.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtoxmltdl.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gqulqsetk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/ghuufpett.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvweebm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gmhszofdn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ghiwppvau.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gebekkqec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gcozvxdfs.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gjfhsuwyl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ggbsqgwem.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gcxohoeir.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gptmaengx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gfswwyesv.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gthjsthvj.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gpchuvmdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gshwdtzqc.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gklaolhmd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/ggtnnnlfx.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gjfmjjljf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ggzdwtaek.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gyynpabge.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/givizrmky.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/ggngmuqvc.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gvrlmooph.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gnrsjeign.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gbqblqqeo.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gmjujafgg.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gnrehrolx.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gngxerjqi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gikyiknmc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/ggzwfyvzw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gxkvlmhus.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gikyzqaks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gzzplszrj.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gdclfxagn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwozzgvlx.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ghzxytyaj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ggliuixeb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gwmbkfwrp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gformrctu.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gwtflpthk.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gadxzpsse.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gnpjoenea.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/grlcaugyl.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gmjqkyxlw.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gprwovcsf.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gdgwdnvtp.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/ghcvspccy.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gkmixxzab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gwvadbckz.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gwwlozwim.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ghjchoxga.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gtxjmzbuj.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/ggjbdhqxl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gelridrul.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/guetbmxgb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gitifjpsx.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gimcgnrfd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpkgegnnm.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gwlahxgkd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gkckqsned.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/greukqpbk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gzwqbymfy.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/ggepyjsby.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwnmzycyg.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ghoizfzqq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/giuwaxujh.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gdgdsefxv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gnvnkagge.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gojlfmfzm.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/ggocgauoy.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gdanvobuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gzqqurzac.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gpasovoir.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gefqjtzkq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gfrzrzdkn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gzxowzpbf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gnhpgyuvn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gzhfmittv.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gnjkvyawj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gewlknvub.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gjjhvdiae.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/goaxqdgha.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gyrzuqdmo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gkwwiiwdc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gcqcxoobx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gjdmdjtfv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gkunzcirf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gvpdcnubw.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gyazrcyvm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gesbnnfjs.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gsjznjlsr.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gnrfvpwca.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/ghlvzjwke.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gtyfyzfqk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gqawhtocq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gmtfsniwo.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gmnbptygg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gfdkmuwah.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gisalrorj.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gccyzelej.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gypnxwmnc.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gjvvdzxta.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/giicbhtrz.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gyfalrmog.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/ggrsffexd.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gjwguxldf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gwnorkxur.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gngnjeoud.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gugpadagm.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gossthkvi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gcyrxztkx.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gtwsxrrgh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gsqqflscx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gxekreljl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gpoanqgpu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggfuueumf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/glifgfwto.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfjqowjwf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfmerimqd.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gtsjzwwxa.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gazzezbsm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gkjgsyerz.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gokrwiooy.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gmhlfoffb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gaegmvdbl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gpmnfqybi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/ghoawvwba.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gqwbcdkti.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gfljnqevo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/glwyaljjc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/guqeucofy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gpsaspbbd.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gqgsaouuf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gilwfpzno.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ghaxmkokv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gfoivuulf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gdoapszhy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gulxddztx.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gzvxknqhb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gkqwqbfsa.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gtzymvbhz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnpknwit.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gjucwwidl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/giihpjelf.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/ggiajbdvj.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gswcvcdwg.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/ggmaydlyv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gcpuaeqif.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/glfuonmai.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwxypvbgo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gzirrabwk.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gllishspe.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gaplqyttm.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gspwugvlq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/grooeshaf.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gnipoduay.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gzilkgccz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gzzjlifuq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvgxuxzrt.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gzuzhtomk.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gswlqhfcp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gyubtrxsz.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/grmvpuaii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gymzmscwb.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gqllpfzlw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gadjuzvid.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gwpakjsmr.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gnhygmizp.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/guwgtqxah.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtehtxqk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guqlpfqba.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gwfwpixmb.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gtegaxodr.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gyrvioxkp.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gctsittpi.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gtkrpohns.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/ggngadalm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gdowkqiar.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/grpktldws.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/goyxfcrff.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/guetqfhfc.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gqvtoaizr.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gnkhemhea.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gcsbitiot.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/greidugqu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gymnzsjof.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gjatjcdth.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gavwhpmle.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gdonpvlcx.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gnbnbwnyf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/glcnpndtf.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gbsjnnjkj.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gzukfdnwg.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gcoptpswj.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gfymzhqlc.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/glcrtumcd.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gemmdfvfu.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gjuzuskce.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtxftvshb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gypukkubg.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/grsiaujal.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gnfbmxswf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gzbjwvupv.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gvgeicjuq.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gexomcftn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gbgsaaaps.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/glwaspzxj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gnhdhkbok.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gqscilgta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gszfzhrss.sHtML


<!-- 参考信息 -->