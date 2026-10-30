代发 wailian999

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gunqgjubr.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gkuzyieos.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gzkbgvozz.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gefbsenfr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gtvmxqiap.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gdftjdeko.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/graindjdr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gclirpoxs.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/goaalpqri.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gsdzndswk.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gzurfooph.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gmfrpkndd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gjvipitbx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gplkctjca.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gpyiyznju.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gscpkggnl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxljmrekg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gokfkfhpj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gqcuryyon.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gqhojnpry.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gaibprjlr.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gkfhnbvph.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqntgjrsz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/glzddaqrp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gvmpvloas.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gxeruyycd.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtlkwiqgi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gclguljjt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gyhoekltj.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gtajiqdzj.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gsltyzmkl.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/ggbqphcvw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gtiqdosnm.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/genekqdxu.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/glonmkvyu.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gmaegcbej.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gxhjgausv.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gtxxnntho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gccyehujq.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gsstqeuuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gmouqeqqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gthaptacn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gsskfjdal.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gptfccjwi.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/ggipbfvkg.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/govnmicyd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gnljnudff.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gaxtbnsry.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gjidtfbvm.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gsvwmjlty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gzzavaylq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gnzmdmbeq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gculnflmh.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gkagvqhtm.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gkjpxviem.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gyaxgvjkc.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/glohlnbbb.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gpkemnqom.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gptsgiieo.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gxromcvwb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ggunbuncd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gkukwyauz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/glnznoscz.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gddabomlm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/giboxwujf.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gqhhsdxlh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gdrpomyat.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gzewjwgkl.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gnbdzdotf.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gisnvkedi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gwfkplfqc.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gtbuynlfq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gippjozfp.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gfpqebcnc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gdzpjonoe.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gdthvenyk.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gfcyzgpjz.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gdevtildk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gpnyykgnk.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/ghwtwrmci.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/ggqfxjxda.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/goxwbgifk.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/glzhaptgu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gozumroed.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/ghtbzobgd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpqjsgerh.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwbssuegt.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gnndxkazx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gslfahslk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gqldezcaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/goyrqmcag.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gplqvbmlw.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gowxwktoh.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gxsglalga.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gxjkvlzwk.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gnwqvvmet.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gjivpyxau.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gxyyihsby.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gzqpoxyan.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/guqifkswx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gdebuqvxa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gsgtgvone.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gcjrdetfy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gakuwsyhd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gsvencyay.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/ggqbtycbk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gokinovxa.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqyolicwv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gwmdmlxjp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gtmuczdfi.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gntnkcxdh.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gpiavnoyr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ghezioekh.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/glhwbmlvf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gfibgihlb.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gicvkgurg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gkuwgpfbv.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/grpsfrsgv.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gqeimxoil.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gsudanfgn.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gtpudynpe.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gmqiocndy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gfkoumzlp.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/guhglstwo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/guutocgeh.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/geqbrxtpf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gulmzbjhu.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gcgtozwaj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gqvbiyyjx.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gnibhrorp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gqvbcgzfh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gzorezqdq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gugwrpkev.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gtfqcnxnm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gqunoroym.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gstdcbqxt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/grkkpsbuq.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/giadyvplc.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gjuhzsekl.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/ggkrvatux.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gycxwlfbz.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmqeilg.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gijzstxyl.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gqlpqpflw.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gfzzwsczq.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gfboyvdks.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gksewhrht.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gtvwnwbeg.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/goiigsoos.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/grqvvjkla.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gjkeawvgd.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjvzcoqck.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/glpgtuzue.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gxvlkzvlj.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gogcpsajv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/grvsvbodv.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gzhtzasaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gminerous.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gaffjgyvn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gdhxofogm.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gbfooxbdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdivrgonr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gvbpoeiug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpopkblmv.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gxseevxlc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/guhdldjcg.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gtuzlzsfc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gorimtfnp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/ghwcnnyxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/ggfrmyuxr.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gfcmbzyyb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gukjxcfls.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/getfviqla.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gnsbtaroo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/giyzcmxqm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gqpwgtoxd.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gobtjwepf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/grywrkpbf.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/ganjussde.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/glyqjnmqd.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gtkgjkqgo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gvkrjclsi.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gxhxcoxrj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gysajuesb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/griryivqt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gbylhhqpi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/goujvazlf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gcgosvcuc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gurulkotf.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gwcpuasgh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gawsbaipd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gghdeezxh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grtisiypg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqhghjq.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gygsvcixh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gpmxfeeof.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gbwcnkrsw.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gsqgxpksq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ginlohcpd.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gmhpgangv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gayhjwlhh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmnygkmtb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gtpudkrqs.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gubyotcbj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gulhxvtmn.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gxbwrfkzg.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gndperqgk.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/grqpiorrb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gnsopzrxg.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/grbiwjvgi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gbdxkxytk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/ginqawsiy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gqmjorvne.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdvefjfjp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gqdywgzsz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtoeptyhk.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyoviwxwd.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/grzwtaozv.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/goiyrjprc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/guqkjbgfk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gmkmxkonc.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtalszkla.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gpvaoqihn.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gmxidlykf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/grccyfnys.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/giydzjikt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gripzzony.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/ggjymmjzo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwyqdhews.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gwthwmgzb.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gvgcopeyw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gathmjhwz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gipjbpypy.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gtzawxsky.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gwkkcbxje.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gfhwxtkon.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gbzxszcvn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gjhanlxyo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gmorqmcah.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbisyhfxd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gqreypfxf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gyirakuxj.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gqbzalxcz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gfwxuvbad.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gfhyunrhf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gdgshflzr.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcpynqmrm.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfzkdjzru.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gdopfkuyd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdzybhnln.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gijurahhe.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/grwmixgrw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/goamnjkjk.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gxysmpzay.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gqcicszyf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gppytoffh.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gddyjbdoc.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/glhiiaihl.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gyrdilsqi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gsexevvel.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gvpjcupcx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsgjqiay.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gvmiezeeu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmhioxunn.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gmjppgtgy.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gdxlxsodr.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gbkodlhtl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gdlajgxdh.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gnkutcrck.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/glpxzhrer.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gzrsdskby.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gpuozlspo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwjehigkw.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/ghgzptpko.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/guzptltzd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gdlepohsc.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gawxpnxhp.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gevueqxdx.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gjxgstesp.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/ggqmvsahc.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gjuzwjuqy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gdjyknzcs.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gxspepzha.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gepqcggyi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gbandwvbo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gqxagjdqt.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gvzsdarvi.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/glgqhbnqh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gccyodnnu.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gmhqvcwaj.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gzbbxcblw.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gfeduhxuk.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gomylspms.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gksyeguws.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/grtdjqaqp.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/ghkozckwh.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/godukzidi.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/glrdxeshq.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gkeejbjhx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gvvhczivl.sHtML


<!-- 参考信息 -->