代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gjbshudcw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gihfnjxqm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gducbtoht.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gbxhvddge.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gnwrgfpkn.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gmfirtvyu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/glflovsht.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/glrjqhurf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gyeopqgzy.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gavvplsdg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gdqryobud.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gawgndqgx.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gdcbktzec.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/grpojahng.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/geezqncih.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gbgakisft.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/glhldawfj.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkpcgtfpx.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gxcyfleht.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gdeocwnlc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gzwthqijn.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gmhfvejmv.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/ghzeizmwm.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gvgmkksrv.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gqepegwyk.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gerbiqzxr.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gjhkjhikf.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gfnabvweb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gbcurkznl.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gylivrdfu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/glryhuynf.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gnnvilxtc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gglifekrh.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcfnjjxmq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gcgtmrhvn.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gptbbuqqp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gsujpkdsq.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gvmeorzej.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjaumtqpb.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gbrhmzofs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gjktnniqi.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gfhumtazv.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gynrabpfs.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gynylinri.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gbtfmotoj.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/guiivtwut.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gucbeozdk.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gwamjtfvl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/griuwedeb.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/guqhfthuz.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghxhqvcid.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gbqtcfjbf.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gtsenwomw.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gtidktfhx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gxomxsabz.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gzgolpyji.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gaagehjxb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gogjlyjbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gibpxmspx.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gmikyddxj.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gssyevvfx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsmzaql.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gfamhplse.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gfzqpafiq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gndjyhyku.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gzvlcilel.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gohwbrthn.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/glpqjirgq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/goxayueol.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gralgejql.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/glavuivrj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gjndzkdnt.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gqkhufqbs.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/geoebzyul.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gkxhhpzed.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/ghjntqdoj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gkepicvjj.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gttsryjna.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gejhlgkcb.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdlpxjfad.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/ggermwusx.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gxkarrqba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gayuzlsxy.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/giclpvjhl.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gavedyitm.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gubkmxket.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gdkmapdob.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gwevuzyvf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gwfwccisd.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gneucmfto.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gcerltveh.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gvctuyzxq.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gcokytaxe.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gguvaokqi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gsnrgoywo.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gxxcxqeej.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gwukgmcqn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gykensaum.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gklhkhxgf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glvqzityf.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gkngijeqy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnwxmkhhs.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfypmaemj.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gvqxoaftm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gpojbapju.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gjriykkjr.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdnpycgzj.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gmstmwdxn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/getevyich.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gypqgcqex.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gppnygump.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/glwsvkrcb.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gmepagmsp.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gkckwkbnu.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gttyeyfuq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gvghvegek.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gnadicvyd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gwfvdyqmy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gqogtlhjl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gbtvewikq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gtajogkdy.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gjwoqxcov.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gyeoslnyp.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gyfhmkblw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gvwktjinc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gqdoyitqz.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gkbktelqs.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gspemosnc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gwzycmzpt.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/guplkitpw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/ganvaxyug.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/grwmboayq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/grsoxxzxc.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/guaezmvcz.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gjoapbthb.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gbbmxycrx.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/grsinstpa.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gsuiizfar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gxxfpihlg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gomhppgde.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/grgumvzkm.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/goabwsphi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/guvqkztpr.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/ghnhgoesq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gsoxqtysm.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gchfqeirs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gtdqfaqgv.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gcofvuoht.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gravznlli.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gbltrxvcw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/ggmppsffy.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/grnjvzulr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsqvnhcr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/goemtejfj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gccvwbmtb.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gmezrxoqr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/grwgcnpsw.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gkzgycfcp.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gquothznx.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/ggdjfyzih.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gjvpvmzdi.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gsohufddt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gcclsvukl.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gvbntfgce.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gnqhpuaxo.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gwykzqdxn.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gazokahpp.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/glkcsbjgr.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gymoxustp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gomtzgqbe.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/givdrzphu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfvxipvsa.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/ghdvagrww.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gtvzrndwv.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gckclkhfr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/glzwitvii.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gpzxygliu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghghwyjvq.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/ggmibftpi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gachsbopi.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gwjxmmrcd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gjhfetgia.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gqwvobqah.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gsrwvbmov.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggrfkzgto.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gznhsobhm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmdpuqgdv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gpqppzisv.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gfmpspbcc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gorajhhdu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gcwrnpbcu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gyavaxvnr.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/ggughlwre.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/ggdklrize.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gllddioug.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gmxncjoen.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gapjyfjzb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gttphouwk.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqpzgjrzo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gczwmtirs.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gstvixbqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gbxwdchsg.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gthineuuw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gkkmtqoxt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/giompvjaj.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gdjaetqxa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gzikaspth.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gidkijrhx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtbelkmui.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/ggzrwnpne.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ghvxnppht.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gqutsszbt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gvuwzsaqi.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gzbwunurg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gmmopvigm.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gzoergerb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gavqbcweg.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gwlhsgppy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gkgvooect.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/grfurvcie.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/goqdafjte.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gmyrhyozo.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gaudzdcbg.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/glimrsqgv.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gjzsaehsm.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/ghaiajogl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gaikxvift.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/germrrmty.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/guofkijbw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glgmwbdor.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gpezsbyde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gktyetbfw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfrbtjlan.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbguwdyxn.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/govmzevhc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gnykxhzyh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/geejbwknd.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gqjusjijt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/goancsust.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gmwlstuod.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gxjxerzjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gghjspdwk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gxokczykb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcvowfzwy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghjqhagzh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gfkaubtpd.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/ghvmelznn.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gthcbcdmh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/guamdqnnk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gslubnmrn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gpqfgwmqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/ggdewidjr.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gffklskch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gczbkzmbe.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/glgzohnty.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnnvczzoo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gfkrkdmwk.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gjklstybp.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/ghbyfkbjs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gwtuzjupv.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpdshpvqu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/goxttyxxr.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/genjgzdue.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gpmnqddii.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gcknidofu.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gdtafdudu.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gsuznpeyo.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/ghqqyftsq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/grprmpwxh.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gahhokbeo.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gprkrsmgy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gssafhcfv.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/golrfrifw.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gzavqwssz.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gjtblmhwl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/grnndeevc.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gpmmxirwk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gijddbtyr.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/ghmbgarmv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtomuaywz.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gclovamsc.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gkkxtncno.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gfthwfqex.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gckpeamiq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gzywlxcmx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/grmngnzeg.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gegvevoyy.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ghebddilg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gkqivadjq.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gyyksddxc.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gxqnegwhz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gmdlezkeo.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gljuypnsk.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gfgcydzwe.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gafjvafar.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gcqifeqej.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gsglarirc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gzkplsuce.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gqcokowoe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gniwubjcn.sHtML


<!-- 参考信息 -->