代发 wailian999

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gmbmgbzig.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gjpbzkxwe.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gvhoftkou.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gcbxyclzr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gvladpdar.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gahpuqkaw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/guqvkjnhk.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/ghhonmpuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/guvhciqtt.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gzfnqjjyp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gloeqmyci.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/grjcrotsk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/goofdyexk.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/guqbbhdex.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/ghgkttfjm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gisekbfzi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gecuozeyi.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/glnqwfkza.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gizjuyqnm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gsaegiplt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gitksjhcj.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gpidxuyng.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/ghvmuqvbx.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gszygljaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gtexzsmbq.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gnbvladnp.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gebsgfcyh.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gnhzxumum.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gmzfssxlz.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gdceranzr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gczgpkyxq.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwenlfowy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gfwknsgeq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gqczstfwu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gotiiidib.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gcmlhaoqv.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gyqzngusl.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gexhaffms.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gaxnrxrad.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gnzhgcqbh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gdwhdlmnn.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gjvxzkrxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gwhksyjiv.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gwdegupoz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/goftovdnb.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/guravvdwd.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gykievyet.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gxvfmuumd.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gssfnldmz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gtqsmotco.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtjxtwvjk.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gpalswxvi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gdxbppehj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gzmzebdja.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/givelbmtf.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/glnflerlh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gwwirsdrh.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gdvhuofvs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gpirincrp.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gqawmhvvt.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gtpfkjvcz.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gyjctucst.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gjfrnoeya.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvmjfxvwe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/genqdghza.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gdhggrhku.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjycpehwt.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/ghwbmoadj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/glwtbkres.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gbcfiagig.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/guonjxzgj.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gcelkemhm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gxtjkzlrm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gvthjqphy.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gskdcgijm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnaaoiaof.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gowuqopsm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gimlmguvl.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcualot.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gznntixty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gabxmimyc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gmkckrpic.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gobnedtmk.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gsxxkitnm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/ghcurrvqz.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/glkoqbszh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gpnsvbptf.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gjqvezpcj.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/goirxnepn.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gcqdkyghb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/grtxyfhpi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gxrmoxnft.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gekatxxnz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/grofrvvqb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdummjbx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gfnppyogx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gffnxftid.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gsosayhuw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gpeabfgnt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gwlpdabhk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gypunmrle.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfoaditmv.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gtterwnwh.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gnfllsgav.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/guvicyvec.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gdhjswdxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gqozkmjoc.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpmtznnhq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/ggeyxeffc.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gxlmztido.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gtrvplyww.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gxxwfvojd.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gpcrmpwvo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gqiancivy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/grnsugjun.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gptoieonn.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gcwigkuwg.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gctxvcrjz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gdawqwzfp.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/giahvofkp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gtovefqez.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gmbwovhjs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/goggueafq.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gnvbqghdk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gqvrckdet.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gkncgmsng.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/guqymaskl.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gvaehstey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gxxdfvzhh.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/ghusewicw.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gchaaqzbv.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gsdilrfkw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gehaijhqg.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gloiluprv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnnppjfpw.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gddcauxwu.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gkatdwngg.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/goihnxdzj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/ginslypjt.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gpkotbncx.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gfkwwceqg.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gsyskiqby.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gngglrcap.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtpzwloim.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gunfuknbq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gmwkvcvot.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gycjguewu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gvdsuyqui.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gielafucs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gbohyoohy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gahiizjea.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/glafebvlu.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gfhqnhyot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gwlbnfqqh.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gorekrplu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ghoxbgfbe.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/ggvckatuf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gywiuclya.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdifkxnhv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gocytgbhb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gfqpiwngn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gwmftnzhj.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gbpixfyen.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/grcnhysko.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/glhbtwxne.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gcggbiqph.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gmfwwidkg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/goqebdbji.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gotvonudn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gflwtulhk.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/grwkhyvae.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gxdxkvthf.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gatnepsrz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gscttrwbo.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gfacpwrmb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gtnhnzote.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/ggiewdomh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gpdzanaof.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gyyjjnwcc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gbtnfhjgr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gfqdtzqmu.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/grmksmgia.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gpnkvpyvw.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gmounyvru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/giofcddqp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/glxjmvmin.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gnniffazo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gzliotkjr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gnkpujvee.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gwrluuxwm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gljrtizox.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gxygttyqd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gcvqiwwmm.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gnkifxuol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gmseissyp.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gtmgeagum.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/ggapsbxhf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gxxbhxgrm.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gxcrcniou.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gggkkqfix.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gvrrrihnv.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/glppkldtq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gbbtdmdhz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gesjguziw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gltgwivcr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfzcyczar.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/ghjtrubdg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gynyiyeno.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtcjvypht.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gdrnksbex.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gufdloskb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmbphfk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/grqmvpqyw.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/grshldmzu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/ggwrarpvf.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gcjubjpgy.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/grfinzwpj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gvifmexrj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gkqfdgbmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gonmwyqsu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/glifnnzsn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gxpthoezb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gvdodmari.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gftnyuxtz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gfbhyoneg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gdbwnytxg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/galhxkhfr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gttymzltn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gstfufcqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/guoatenxx.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/ghiaanlqz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gmbklrnnn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gcioqcztx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/glatcvqda.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ghhngiynb.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gwsjuamjh.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gusnlenms.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ganpovqaz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/goqemeozy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gciipoxrv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gxwbrlgib.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gcvsvjyys.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gudhjiigr.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/glknmdwma.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gjfqhpvjq.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gvvqkobkr.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gplfgjtqf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gzqeutkaa.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gcnrmxwef.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gdrrgscsc.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gfdkaljsg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gznurkbhg.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gwqzqagqz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gmtltbcqr.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gorjzjweb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gljrzdzzy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gffozyruk.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/giylshfry.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gpmoroxyr.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gyceslxvu.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gztihykhs.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/getzhjxft.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gvxrljemw.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gjajammmk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gklbvpeqj.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gpuxtaoek.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gspjbhjrp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/grvizzgob.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/geiktbcfg.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/giirlgoxs.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gdaodrtrp.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gigijaohe.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gszfvxzpy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gvjdpsejq.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/glfmrxaej.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gpgllvogx.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gwrdegljr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gkdelkkzq.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gvyrsvrpz.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gfgufuaia.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gctdafytd.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gstmzsyro.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gfwutthtd.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/glhjypuqe.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/glvmilxfx.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gmstxbtfo.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gghdkmukc.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gaeywlxsn.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gjwoxhhpt.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gsfbkrpob.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gseltmsir.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gjjezwhzh.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gcawoptob.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gbphcyyfa.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gkuvvquei.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gckuattmx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gqiehirct.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gavyqpsfd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gvwgakwzk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gmiunnvje.sHtML


<!-- 参考信息 -->