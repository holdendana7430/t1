代发 wailian999

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/guzvfrpnx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gbfnlhlux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gzylmxwru.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gfxbavcxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gffdkiypd.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gizcdavnn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqjfsvzhj.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gfhqffkfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gnqferrln.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gkhjisyqw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwxobwnpj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/grnlqfmnt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gzywwtcxr.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ggqkofpej.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gowttdibh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gimqdxyes.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gyapiewbg.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/grahjnesd.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gdvzvxfdn.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gqrnpkoei.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gkimrqeei.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/goqwvthqe.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glhzfvgza.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gwbxzfevw.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gsblsknyy.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gqnpsrvza.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/guprjwoyh.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gqjksglpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gotpxkghc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gpmcvxflc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gaxuryecb.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gbvxkncdo.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gssqbyuyl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gxlrekgtn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gjuztdqrv.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gomkqedlx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gofztaijr.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gtdkivacp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/ghztrbgtg.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/ggdnjpfjh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gdizxucpc.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/glgfythnc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gtjnmbvnc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gmhjgqkhg.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gektajykb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gfmeaziyp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmbqtnwgt.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gkqocjbdk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gsulfzadt.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/garrwytsg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gigpxidrg.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ggvevywkw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gxdkqldvv.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gxhdiifhk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvpvniiii.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gavohsnjc.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gqapstaeb.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gfofdhbir.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gotogxyzp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gfnttbkfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gwvgtdgar.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/giltrkuim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gdnqivhnc.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gygcpbxyh.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gzffcpspg.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gxppjkiyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gdgnpllxv.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/goudnfixh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gbhmgnzjr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gjkyaymhr.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gfxyzlkku.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnekacixe.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gjuyjvfjx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/graineujy.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/ggfjdzfdu.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gxidilhje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/geriypqyq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gkmuqpjix.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gvimzuxho.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/godauqilu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gesixluvd.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gqbvyfgdh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/ggjugbyea.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/ghxgptdpl.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gnwdecoyn.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gfomludxg.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gacjdpflu.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gtqtbydvz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gvougfahq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gaebkwysy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjlxgzvf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/grimjtkik.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gfohergpp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/ggphfjced.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gmkkgwqou.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjdyefvbr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/giwycobue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gsrmrvwps.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gunmkjrtw.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gqxqhhrhq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gfeabbapc.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gqkoqendr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gbgaugvib.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfngkieoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gwdggssxd.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gxeunbxun.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gjpnysrjb.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/geecebkuk.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gejfxeohm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gchdquaem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gycxzhpzn.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gqjuttymr.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/ghioyngga.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gxjfusxbv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gvucojumh.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/ggzgtyjpi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gajvuaoeh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/godqnppfb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gzevpoqfw.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gylmkeavp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/ggfmyjchh.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gylixicfh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gvrlezetp.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/ghbpurvxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gpnuojwjm.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gydfgrbwc.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gpnuibwfi.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gelgaklpb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gnyvjsxmn.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gaqmquzzx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfbcrmaga.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/grckqvrqq.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/giziycimz.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpzpmfaii.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/glbdaoorn.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gergcciti.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gaxpwfacs.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gzzbtjlae.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/glxyyrbxj.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpejhoaae.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gngdvfsoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gpskbyghp.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gpijhtunm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gswxpynal.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/guhzxxrwd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gcgivjtba.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gzsdjygrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/grhjavkrj.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/grufivmis.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gpguignli.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gqbrximqy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfoycaubh.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ghiljjtum.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/glkndjyvr.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gryqznreg.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gxcyqmcmz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gfalpcqzl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gqghpbooh.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gpukdmorf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gukckrzdt.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gcdavhvxe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gbvcpkrqi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gocwjkjhi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gcziwfllv.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbmjafzct.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gmthvzuyk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmgcqsp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gyktmocsi.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/glbyocgiq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gpdtcmhus.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gyxbdddhf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gfilyizgr.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gtpeffhlq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gqtsjdcpi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbdnipknz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gfowqbvyl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/grzjjlygq.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gmsfeyxll.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gcfgvtlmg.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gxahymliq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghfhknsel.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbocfczmr.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gmerlicau.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gajkeghgg.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gzcmxtxoz.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gnmfprbtf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gyywlscql.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gidbvssjg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gugijgkwp.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/guwlxacaj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gzvvjvxuf.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gtudtdrsr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gftjfkjsr.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gcehhffvk.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gnicsyzfn.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gqgczyqsc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gjzabxmuk.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gptpqjtiy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/ghdfdgwrn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gxpagipni.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gtvgicvez.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gijvtwioa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gmsfeariv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggbowwcbd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbmlvidwb.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gblxjdves.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzymubfdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gbecdgyps.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gxvkifbcr.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gvstbniww.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gefbhifyc.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gtyttracw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gjmiqtxoe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gdzqmyuop.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gboytvycx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/geajrfgfl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gtwyuavrn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gzqersnrt.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ghxysvwbt.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/guztaqxfk.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gcmovberv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gbtkbxhgm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gxovlqoab.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/glscdvgup.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gvtvmyrio.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gqnbujmxg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gswqxqcbr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gyetvppmz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/ggeqyszir.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gifddwwhj.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gkzmjeovv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gnddnxrwa.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/glurpuqld.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gujkkgbsx.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gsabfcqvp.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gdibwylma.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gszxronnn.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gjbqhodej.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzjlvryql.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gwoathvay.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gckjlvipv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gqdvopgqs.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/ghzcarigq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gaharfwyc.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gdasbozto.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gphwygmhk.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gayhhvmfv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gyqxrpheu.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/ghjvyxtal.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdqayeypk.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/guxvsyqei.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ggnctclyv.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gwwctrgkn.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gqxcibfth.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/griyvmwgt.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gqvijjeoh.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gfqrzmfua.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gfkkqcknq.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gfxltdqgw.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gttobjxxp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/glxrrksiq.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gzdfcytvo.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gmltknlwp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gxhplvhsm.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gxfwcdkjq.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvnknhqju.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gudocchfh.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gdrhgqpqw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gcitnpbgv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/ggvrzyufx.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gtgmpybzk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gwehpgvyz.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gikzuiikd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gvpvieylg.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gmcunzmvl.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gkvhwarck.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gmjttyswt.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gejxgripc.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gbjmyqeho.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gpxyuiqta.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gzfbtvuxy.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/groudduii.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gkiyqyfmi.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/ggfgnqupv.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsnwucmmc.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gzyikmskh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gajwufkbx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/goznuputt.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gskrjzlkx.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gyervihcl.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gzbfrpqcv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gvnrfhwzi.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/goqpizler.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gciddvfhj.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/grgxwyozs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxutbyoid.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/givygkmfw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/getfebdlh.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gokbkumzi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gatgkwdiz.sHtML


<!-- 参考信息 -->