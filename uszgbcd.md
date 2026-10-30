代发 wailian999

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmguaksm.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzdoygzx.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gknpuuekv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjvnfyii.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkupwqmbk.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gljfhrons.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpffxbfu.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gslwcvhck.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gizmbsgiw.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gppqiuiay.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzliiybfr.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/goliezynd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gagouhfag.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzokjuhzo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyftxyaab.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbcaxvzo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmguvncr.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gupjcxjvf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gswgnooek.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gffykzwey.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfndamfm.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhgkdcvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnpotmfp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrxfnunw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gclzajxtk.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gujixdsqq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfwofjdo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gdqfhgsip.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gicccqewm.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtanlsums.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gubssvoia.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gfeymemro.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gvedmkytn.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpwgchhu.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gheprkxqc.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmetsqgf.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gbnrhpqap.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzyrhar.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxrdtfjy.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnmerjao.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvmbozns.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpgwbahth.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyhpwqki.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrcjigum.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gfljqerwa.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaeaqjbty.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgosjpdy.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gkkxlbhyf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeriyzsh.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gxjjljbvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gimpdzsiq.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gjpwdchgu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gxsrouqsi.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrsgwxyx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/goiftumbc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gmxonljwm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrvnqeqi.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmgyujjx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadtseohj.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/griwxlxty.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxppruwg.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gdojcuupo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gsamoepsf.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gecauhzcg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggccexnya.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfbcmvbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwdhcztdl.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcikvzhyr.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gyzggacks.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gkqbgnivs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggrsahzxw.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwengaund.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gscxglsdw.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glfojroin.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grfvzilkw.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/glbgmtrno.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gleqwftja.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/grzlnkugc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gekmwxcep.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtppotvu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwyjpqyt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqyywkin.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkhbieos.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gygtuqkin.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gillqxigk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grojwwnby.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsqzmbiw.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlsikwoo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzarjyode.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gceiuccyj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glaqbvmgo.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzqlmxin.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvnplpvm.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gmkiclewb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/glwywjbak.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdzweiwr.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoyuuzky.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzqdzdck.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqwuvgxq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gddmnckhs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gqukrszzt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gnezvpdes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxmawycl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glfrwcrmf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gkbwntevj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyotanneo.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajtlovri.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmphquvws.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzlwprpk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/guoqeaips.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gxlwmomfb.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmjznft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glinsaonc.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyztvikd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/ghzsjzexv.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gofcpnnce.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gciatgzkh.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtxqhjiqk.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcdrcyjht.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvyfghy.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtmkpxbv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gztbvgyof.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gpoynnjvw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmllkwyde.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuyzrcjb.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrjzqeja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gojnpuuez.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gyuencbbl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ghicefxrl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyxlgpcw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaejxstv.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gpskhaaaq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/glgojtmtq.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdwyceyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqseidsnl.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxfwccxe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbdwumkd.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpcadfst.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqjkijte.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/grbsgivvl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gnhayfihj.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gcmbnkipi.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gilfsuihf.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmsscogw.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzclgzabk.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmborgagm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnzzfrrj.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gssttfnqn.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfgmsfpx.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gpygiirty.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmyliatt.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdsftkyx.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnliufgbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmwlvrj.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwqppphtp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqncinokg.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gjmcnvgby.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmgtfknd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gekiksteo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgpihfxx.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gdnmyncrv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnorycpbo.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gkyvodixo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggunuxzcy.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjnfbxyc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgkmswoe.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gchpejevc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmtxdfou.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpzatkcwk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/geiartlyq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqcfnfnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohajzsaa.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnmjgaltc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjwcrzs.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhtihhaj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gveudxvjp.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gmbshfrqh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gslowqgtc.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gftwtcwjc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstfoauij.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnmusmxk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwzpqiump.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomldwvys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxwpvwnd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwqsrglam.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guszfaefl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ganxxjjbc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gcdaakmnm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gknhjpiod.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdbukolok.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glebbnfre.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjkgmwgh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpocinsf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnpzawzc.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbswvwikn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/goveeqdsm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqvnyfequ.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gvnitlmjy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giconrnjc.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gsysuaiez.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gameruffc.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gapgojnov.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuwnlvcb.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golymlggp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdvamzsj.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gywuoyeat.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwyszeso.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gouhxvojc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfupqlkmq.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gouwdlbtj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gkizhgokq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gicobhzww.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapdrsvfd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmzjqloq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gfryfntly.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhccklmr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkbkayavk.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxwszgjs.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvxzhpiy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gokkyymhf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gxetzjtmy.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmpqmuqrt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/guatiivrk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdexikwn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqpsnfev.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/getybqisu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gljtwzumw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glhtkxusa.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gldgxnoki.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrjufzug.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghribfzno.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzahoxgh.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gevbfoftj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gntobvaxm.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrxzjfks.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gvpiyafre.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghflcqrij.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtxfwiqk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/guqcwwcvi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwmmray.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gcllsndpz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzgtqoqn.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grnblyoie.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykgwgirh.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gykkqfldx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggxgfcus.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqzcuhkq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/geyuluuop.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gntmalljf.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhkxemgy.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/galaubwhw.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeeyfzsu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuvbhqbj.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/glciqzkgk.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grehqnjse.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlwrpfh.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gluddqgvm.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwffncrz.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gggsfbvpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxjnryhn.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glhlkoiiw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjoesbo.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gltjzcgbm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/grkhryczh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktrgnyea.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gffwfofas.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjzjyvcj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlyvfqss.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjczctceb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdjmmsysy.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ggxeggqvb.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gdodtdhyr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyzksgvu.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/ginwcrkvf.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdseltljr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gcprjmhaq.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjooxxifj.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grtklybvp.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjyzvgliu.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gynqkjdym.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpglenub.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkfdncpg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafwwbzri.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gtshztash.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbxmwvj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnisxwm.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gndnogiya.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gbglzwkjd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gdehtthrh.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gelbcqjgc.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpvtfbtpg.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gsddsgtkm.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtfguxqwd.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnskvtiic.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gknkfxljc.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gcddjaatw.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtfiatobp.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gyojbrata.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gyuprrqdl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvrbrada.sHtML


<!-- 参考信息 -->