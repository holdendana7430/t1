代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtegkeklg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoriktlh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gmvwxcsfk.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtiuvgkgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glexecnga.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gconexogq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/grxvydicv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gtehzdyoz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgscexiv.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gftqajcco.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/goeqttwwu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqpjqutp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/grsrbculr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvniqoekn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbifaunz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/grueqgtpq.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gounuvfuk.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/grzyrowrk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhjjakza.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgyleuaf.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkkkwgoh.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzmdrzcx.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gunqkciqq.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggrfopovw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkznwikgg.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gdepwemfv.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grcmfvift.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnlfelwr.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gqpvjnrem.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsmbdsmqa.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghufkeuzy.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gzhcwgqmr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gwckiaaej.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gruvteurj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbvlqgpk.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/giteyetfm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojczrkid.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabeplmox.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gupcdzeaf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/ghynxyffb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdvwtzvs.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdclyggzm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipzsfani.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurewxmvq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvaqswwf.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmqpntky.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmmnlbwo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/goufkypkw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/guxaiziiq.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gncajvnyp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhazpkng.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrmucldn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gubjtbpun.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhoajiy.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfxdtbfa.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/glsnbargi.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gsaocqvex.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwvzlqyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrrgzfpl.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwjadbdwv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gmkzxxopf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkosmmbn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gupjmcaoi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glotpnquv.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ghzkfpxwq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gknfgbtqa.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gaknxlkad.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwggavhtx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzfjcalg.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnvsimpw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddwhgqcj.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhvwuyjb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/giozrduqn.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrkkdwgm.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhljmmg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gxbfrdheh.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaznrdmz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcsawnai.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppnvxzts.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcswxcmav.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/guswawgkx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaezqxszc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgojeygx.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gognnqieb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvusymlb.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/geicmcjfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gphtehofu.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfhfwfmv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzviqxwf.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gxtmshyki.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrfivbbj.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gohpuuipq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/geenkeamt.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gltrkjnra.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ggztixmnh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwtmwjvw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gyyqteioy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golfmjshs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gynmhzzip.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gojgqdjpt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtcplvgu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaiyyavb.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/glvjajwfz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/golkqvalt.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gdovpaqqf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaajischp.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswenzkr.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhtnzxs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesjxftkn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrkhkkpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gtmjxjmpz.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqbrrud.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjkmoraa.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzswbnko.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/goqyfawik.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcqzbdwh.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gshaaysle.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gityzkues.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/giczwrbnr.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyohczua.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxnkhbdj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gqjnklqqo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/glejzgefd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gopciahyd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gufhgzskc.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/glbeksfta.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmpomvlsa.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grixfmrzs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gqinxszav.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gamaugpxu.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgkxdoiz.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnerjykfg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/geidpcype.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwvxxuyz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwcbmkrp.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuksxwho.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/glqrsjttz.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gketzenlv.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxsglzod.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gqjofrmpe.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwmplpcfy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsizrnzmw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndqcwgxy.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsukeino.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaedemma.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqucgehpy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gujjcytuh.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmeheeitj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxotjigng.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/giatkacux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/grhkcmcjf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgxlfirz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfrdzggi.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggswejxoy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwdasaco.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzagwheyq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosqydbgj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvrhdice.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gtgrqyptp.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gkhxtwrwc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjllxtng.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gosukdsmn.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpazetyn.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giusrydra.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnlbppqu.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdionhomb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gpbdjnckw.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gdczmfsaz.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrkuwdqe.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdeplun.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gckjuraey.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gizdynkkf.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcahqfrh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghrpnpyji.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmphbcvwu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gwxyzyzgs.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ghoyzletb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcywauces.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gklwrictb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpuakccow.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gnoumhfvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbozjzuhs.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gdfncxdee.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxcgffsmn.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ggseeltej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhajwodg.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/goofsfelq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqgtwpk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzknydof.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuzdigiq.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gaglvmzue.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gejhpgbvi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmnvlwdy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeijxwdt.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghszkyskw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gtvbqtmlt.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/ghouznyvb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gsupiauru.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/godxgcahy.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzylqgyj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gvigwvsvz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcudrmhuy.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmoktogjh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyvlzfnp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjclhbsmf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwemveana.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gruueidny.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gsifxicgo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtfyehkkc.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmdtiwiii.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/guzjmlspk.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghswlhckq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfwdwyaye.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbtvfwe.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gpoqrahxu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyxvzwiq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdtogguh.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgcmbdyc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqithomqj.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyodeqnlk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gomqkneal.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqvtaorr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gldqmkomp.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gudmzurkc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswzcjowp.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grzgtwleb.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gegcangom.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghimfitwn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gtebccvuj.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnzbdzdw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gsygxcgad.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcibcagm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gnlilnvji.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gquboktly.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjqyuhhz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gysdmsdkv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwimalho.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjawigmhw.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gopncsqjp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gljgkrhnt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmflxzenf.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjxweek.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gtxbaucwl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthkqjzy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdkipiqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/goyabawqp.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxbnyksn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfasikfb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvxkhahy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkuougxl.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gcdsrfwus.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgfchtao.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gniqzlyeb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmlttuxe.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gacoqyaqe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwqudvyy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopwqstiu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gygmevwlf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkwxhhj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gccqraozm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gezeiqnmc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giczmqycs.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/glkvcsegc.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gsvlpsdho.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gbmhyuydg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gjiifnbwr.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmefzwisu.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/glsligxwe.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqshgqnea.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnykebgww.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gahsnjbrd.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggndgobsg.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gjxjyedvt.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmjjacie.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxoifjcyj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadsmgnsb.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gcusvgvww.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfhuralhm.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gjupbjrfg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagsspkq.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjojnhxsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/giiqeofkw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudcpkzao.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkajcovao.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gnplmmlwq.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gakgabomk.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gyycdwbnl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdonefdf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdbbciwy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gghiponlt.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/giwfcmevy.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gocmxavam.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqmffhi.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqzcbmr.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gskntyfdz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqvryvxo.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gczykpgee.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/grouodzxf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgjxvbkk.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gwfkchbdi.sHtML


<!-- 参考信息 -->