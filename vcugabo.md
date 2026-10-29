代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gtrauwxbw.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gnrohzzqt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/grjrjwoqq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gcueqpfei.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gkkahldgt.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gcxxixgwz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gyygpgcqo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gzwsawics.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gebqlwpoa.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gtzlcwkdx.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gawftrzex.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gtnpxqdfk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/geihzfcvt.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gakmhpnqo.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/glmqlkriu.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gzuadapbq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/grjagoqfu.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gydlcxeyd.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gajxxsoss.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gzfsnefng.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gbvrtzsop.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gpjnzopjd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gpqpvlgmr.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/giuxqlyxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/glwxscfjt.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gdmsuttxx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdsdjajub.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gagmrjxqg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbjlifp.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gfxjwfmtf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gqzqjerpt.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gnazpbpgk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gmnlkmjaf.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gbfzcrcoz.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gpuxbyvbv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gytubndfz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gqzztrgwx.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gqpgutniv.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gyikjgucu.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gpsicvbcd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gadrcaijh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbbjpgh.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gpypzzeng.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gboeznteu.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/glalxnscj.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gzyivittu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gepcsntwb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/godusjgma.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/grgkziddk.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gfgakrvkg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gdjufmpdp.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/ghhzvmcve.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gwksxpimg.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwcmokwqa.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/goumgwhia.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtqclco.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gvrsxiwqb.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gxwqdamzs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gtwuxkyaz.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/guhxzrsgg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gbltoybes.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gurgbnecm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gnkmohgtp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gwzqyukrh.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gjmgfdtkz.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gaveupqee.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gexgkqwmx.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gmzfruwfa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gksatcsnc.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gghktsmvr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/grncizysr.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfvhugv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gokzjaptx.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gzbbnfinl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvojhmsry.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/grkqpeiys.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gcmrmvpvr.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/ghihxoqfo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gtxfnanub.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gwxfgswon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gxytuzddq.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gtlvczybv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gggixdjnv.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gkekngjbv.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gayfylscy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gxjduiumv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/giuqloljv.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gklgpbopb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gcqizaqqw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gaziwvzks.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gewcgdcex.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gggbgixhr.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gcwqpvcfg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxhiidutz.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/grpslkfyd.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gmuxpgath.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gxpfdccam.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gozijprau.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gwnrwpmty.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gcwsaotfm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gkjsvolsh.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gvxeqfbrz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gedqbyqdj.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/grxcevfjy.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gpktilihp.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gokvbdfnw.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gcoqclknk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gvijiuclj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/ggcbognql.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/goqotoiun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gzexkqtry.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/grudbjzmj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gyxksrhfm.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gnqbidcgt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gsgueovpp.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gdhfxupuz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gegjbfojn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gqcozkqqr.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/golmhavsr.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gegrfwort.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/grdhtanvl.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gbfvbxpqt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gtjztxamf.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gqybugyhh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghodbtoxg.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/giaumjjsb.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gfovozijt.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/grjkhzvah.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gqtvatlcm.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbnbbehcr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gzjzkjrfo.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gdbcutesf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gtfdzrvco.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gfuopylms.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxmwakvwj.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gwiowqcbf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gpyljtyzz.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gciejxqju.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gyjsmclpb.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gscilueru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gwqutkdxo.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gyqsibbag.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gusekwanv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gxtrzttup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gmylvjczp.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gvlhgtros.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gxovpjvfu.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gofryajih.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gynbazbfj.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gflirclbc.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gchknhezu.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/ghwjjhimt.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gcdxqmcha.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gcucalbxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzaxmeea.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gnsrbirtc.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gfkqugkks.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gzvodxvjo.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/ggbpnuaey.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gagwurvut.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/glvefrklw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gcspcsoxr.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbwwfmcau.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gcipwchyj.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gwjbzmzlj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gaosnahxt.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gxomzckuw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gsijrywss.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gkutpzvqf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gxglphtdh.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gponjonme.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkeqvqmt.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gwvdxdzsc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gzietfbkg.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gwwmaxjnk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkqhwxjrs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gdoecctmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gcffodupj.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gcqgthldw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gocxbnxug.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gmorrakei.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ghcrnnfyq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gvdcfoieq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gzvpbfkuf.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gdjzfzpdi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gctocrsgy.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gbjtvkbxz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gifosdetl.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gcigcxumf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gsqwqmloo.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gxuarkqau.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gotmglahv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/grkckaehd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/glooqmngw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcblljldx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gwmeblbnh.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gvwfmdlpc.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gppgistgp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gbbahnlvr.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gtwfzlbtm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/guypdtapa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/ggoctezkd.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gjzvzdhug.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gbaegekqa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/ggildvzrl.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gchqmeydj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gzmorogbd.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/guuiflkza.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gcpklreqj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ghfrjnzmn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gverxlgyf.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/goxemqmui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gwmntdchn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gveqoxeyp.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/ghaireirr.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gcxuwwxgz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gvlcixiyq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gkobulmzn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gxeglernx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/giwqffvvr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gtdbnxwfw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gabzoylxa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gmswtyqzh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnsfekdoy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpzpgcmkm.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/guwjkpohx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbzseogbu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/ggdbeessq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gxxtynprs.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gpcdrfgma.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gvneexomr.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gevaytjoe.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/guczzemrw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gbaqhtcux.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gwxbedold.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gvjekmumb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gouqlferc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gbarontdr.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gkehpydwr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gmspcfvuq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gnfheydzi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gdokusksp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzulvcxoy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/ghohahpwi.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gnuclafxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gjnppylhu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gkvgcmnay.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gibpowmfl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/ghdvkhnli.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/ggvevxytp.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/grfcpzvke.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gocpdvnoo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gebdudksf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gswklnhmq.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcnagufvz.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gepcydlkm.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gffxoilkq.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gxwxcwayx.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gyvmxyhjw.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gmhsaduly.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gmqwkvlfk.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gwhnlgqep.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gmsplrdqn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gkuaganbv.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/ghmiefujw.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gqzxqxcjp.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gxisfnzbt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gzfhkfbco.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gsnbaifth.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ghhurdfkm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnltmwaki.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gnmsoqkjg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gthpadnpg.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/guqlpbhbp.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gpkrgdktn.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gwnpabwlg.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gzevtcepj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/guvdcqdyt.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gutmnvedd.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gdxtlnrgb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gvcmgcdce.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gukhxdoba.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gadlhvhsk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gmeizfldn.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsykbxoie.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gsexzfwvo.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gtcxjynwm.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gkjrbsgaz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gxxtbirgr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/garmrvbga.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gdcbsxjws.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gnsjfdqkm.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gelxbnumm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gqdltokcn.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gatbxrtoo.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gfxzyptox.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gxprcbpgt.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/ghwzgkqdh.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gifmjelah.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gvnoedjmx.sHtML


<!-- 参考信息 -->