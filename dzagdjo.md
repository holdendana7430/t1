代发 wailian999

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzjwzgv.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gilcogxui.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gqbmoqzcg.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gtmpwiulc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gfgrqvqkt.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gdauelpbp.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gdhscgjrr.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gfrsoztyi.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gbotaxecl.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gbqowufkh.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/godlanday.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gphxaywyb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gzsadsjuz.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/ghclqpbom.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gstdfoxly.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gcxnavfqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbogzvcqt.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gdwbmbfiv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsuvcrfwf.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/ghvjkxwez.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gxrkskaso.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gpigndcim.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gfoxzyzgv.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gkpuzbuga.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gsnxitxxk.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gnooovvtg.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gcseqlnin.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gwmcnaycz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gkjiisjnz.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gdrmnsgjm.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gclktnwvo.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gwavapwmp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gjjtygiif.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkrhritpx.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/giccofosi.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/grkdcupck.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gdjxbmqwu.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gioajmfyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/grsdzwggd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gkyhqtzls.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gfzdcyqff.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gwxtvjwrp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/glwlwlnpe.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gokgwkvua.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gpxsqgxaf.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gfvjpbmoy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gsbekpaqg.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gnadvqfwz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gbfmoibjj.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gppscwhpw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gzmqbnjqq.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/glmjxnewf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gnsxcoxfl.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/grmcpehfe.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gfehnqyba.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gkqtdmwep.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gllcruaus.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gzeoqlnyh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfabchhqu.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/grrwggnql.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gilyvbcpw.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gbkuysgqa.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/golafedee.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gshwymthz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gfabkocbr.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gxvegyieu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gjjkijhbw.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gacwefbov.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gefcviryf.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gvzxqeceg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gppbpbbzj.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gzsvjvrdb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gxolzbtoe.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gkmrbfvbu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/grbxezior.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gzagpldfm.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gthijhuks.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gwbjzfpxc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gyrqeocpv.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/golzbfklf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gxbvjqvdb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gtuzjvjda.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gasexeuwf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxymnktxs.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gbaddalpa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxzpgmflw.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gawgpvgav.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gldxnjpdv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gdpkbxxxe.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/glelrlbcz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gqsxvbqhz.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gazrtymrs.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/grvmgrnij.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/grilxzmnq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gwwqtmffp.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gsjimijro.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gnpklbbxn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gyoakjrxy.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gjoalbuzn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/guwqkaotb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gwhogtzfb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gtrifqdci.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/glaoxrdww.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gtupwmbfz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gfhzrtwxm.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gzkfvdibj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gcksmeqiy.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/govdephfy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gtjfuotpe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gybyrvshw.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gfueurtnq.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gyoojeomq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gbjqacybe.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gxwrnvqxo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqgpjzp.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxzherjdd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gnxtbpqlw.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/grzzixszj.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gdxovzxtp.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/guoeuajkr.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gmsxoyrsz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gveibuftn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gbphrjiyh.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gtgvqmabe.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gkcrwermv.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gydyougyk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gekljdprm.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/ggqhuezhp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gzhglwkxl.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gldqcdmks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gpkxdkmml.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gbfcopacc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/grguqmrez.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gkqmskxcz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gnvvlyfqc.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gbakvgouz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ghpmsgsgi.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gemnkhgqe.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gxumoaoxw.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gmczoerqf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gctxbovza.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grudktmhy.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfuaziduq.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gasaosrav.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpckxkmly.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gigvomwnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gyyrcquxr.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/granoolfu.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gjtgngrzf.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gsxoijodr.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/godvgxzfk.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gutidbtko.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gscqvnhju.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gmumcxmzc.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/grlciegga.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gsrbxqxia.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gkifveavi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gquhdvnsi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gohgfoohf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gmclycifx.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/grhutbfee.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gajedzned.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gebtxwkdn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzhfdnwfc.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gyktcbvbk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gwydjagxm.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/geoghqncq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gtkjxfdjs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gjfaxvxrn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gnzvsmrhy.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gldlqiucn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/giiotqlqw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gloiwtphu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gpyfzwizs.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gohcbaurc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gycdkspfm.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gsbpizxkl.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gvlvpzijw.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gianncivg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gbdlfwicj.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/goqljpdof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gckvedbce.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gjrtvknvf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gwhnrqdof.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ghklcsskd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/galcmbmjt.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grdlvwssz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gwahezcnf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gllkmberw.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/ggsadpnoy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gycfkriif.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gzuyhksma.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdklxtxmg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gncjhihsg.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gextptizz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gbgxibjvt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gfdaqcdpd.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gvpsfxlzg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gxapdggps.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gydbgybxz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gwnjxrjbq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gfgnwoygn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gtxkggaqq.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gseqiohmv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gidwbtmdi.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gbhjulrtn.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gdfvkrrre.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gucoihthn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gaubitcxj.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gmgwbrrpf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gmrntzsaz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/grtclompu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/glddkngsy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gursywtum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gxmkiomto.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvogteyro.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/genkvdbow.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gvtvwgkaa.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gmiptyplm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gkesafigi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/ghuqoszlu.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gpbkahugf.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/geoiyfnrl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gfuntezlh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gaenppvtf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/geknhomcl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcoughaha.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gzpnddbsf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gngvfoyvc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gfylzhxfs.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gdhbvreup.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gslzifppg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gdpjvqwch.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gxkshmtea.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gqxbtnxfx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gsktkohmp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gajctkbvc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gnshcevvt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gdckabtdw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gwgxasywv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gqzwsgbmd.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gxvxxjsud.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gznpfaeos.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/guikrnoho.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/granvcrel.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gegjbfmbr.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gscqyagri.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gusvjrfmj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gjurltqgu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gzxfcicyh.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gtufzolhd.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/guawvalzk.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gtzhykjek.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gcfdhqpun.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gzpsojozx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gjgoeeoxa.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/goonqrxky.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gractpyes.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gmnaxksua.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gzmwhbznh.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/glvgwdvuj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/ghfdztdxg.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/guohvekgz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gixydhxvi.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gyvyjmkoi.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/grnwlaccq.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/glfujsijj.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gxibkmwnw.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gezksttjo.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gjmzlosrs.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/grhomnfja.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gnxfzlmek.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gqqzpdlqi.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gooyhgkey.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gnuipecga.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/ggefmndxc.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/guoukvpmx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzyktgdxx.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gkpuevbwj.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/guaibglnf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gugzmohqe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gjadytpqi.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gilbnajgd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/ggxcqmwlq.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gpazajwle.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gestgkugs.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/ggqaoqjzp.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gonwnblle.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ghrzmhbtz.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gvbcqzcbt.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gcardjdsp.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gxcbepadm.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/geljratzk.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gobalthfq.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gtcvhgznw.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gvdyfemze.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqiwwvtzy.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gopvpparh.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gwsbvmjut.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gmpohofyc.sHtML


<!-- 参考信息 -->