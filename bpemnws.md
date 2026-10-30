代发 wailian999

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnytziimr.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdblujiji.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkofraqh.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpsfdkjwn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmqnosbf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsiczpbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gfztbscdf.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdpzwrtgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmscshdht.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gjishkadw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuqfanxw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gctqgfvxo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvflwjsm.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gurejojiv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpavwcuh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupgrqphd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmokvdqli.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzwvcsyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/ggauogncs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfahgrhy.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjebtaebp.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphvrdscd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaufgpto.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdtbxbhby.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gimeoyfam.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqolajtas.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/goixeqdkm.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjgyinjkm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/glhkthgye.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhpepyja.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/godqqamtx.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnzruety.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyjurxyx.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gujgmslwc.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxcmhpel.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/giyvemzun.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gugappwhk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieqgropr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjzqasja.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxpeumhb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnymalsks.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gwlxmadjm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjvofiqbt.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gijwekpku.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgaxkzc.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gyqrddxsv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghatniwrc.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gasybjmsy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/goarwierz.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdifxnlj.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqeqqokhf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gkvigkixq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghferijrd.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gybchdbna.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeahznbl.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gdefymxoz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gryxslasq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxzaqres.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gjjcarjjp.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbpxhjv.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/goybvgxhd.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxohkwmy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxvrzeni.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptdgmds.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gqsbyyyat.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnheoyiro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghhgpgkky.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/ggerpquxz.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gagxhrwzg.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmtmzjwbg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/glkqppiro.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/giroijuey.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gbnqzsswz.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gonbjigpb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/grhepkbrt.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/grdylfzyg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgldknld.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gevuolbbu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcxdwuls.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyczggmu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqtphxk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjtsuqye.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxhmnat.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gripevdce.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxnzaxhj.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gkxvqdurm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgurglma.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgowcacw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxrkufkq.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gasjtadia.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsndmjrrn.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplryfcdh.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gfnwabggc.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdeznobz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzenhfgkj.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gddtobyxn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdflnrzxc.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdymqeucy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/glkirnicr.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gcvvhrebz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtruqmqx.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gklyectec.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/glveayrfc.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gsbhtozah.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpkkyxjd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvvllwxp.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfwaeyrw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyoutfnw.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhhdkuvp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwrgjmhlh.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glyygxqwx.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoqqacne.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstagjvnp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjetahrsq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqbbqkrq.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gqufaxnkr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxitmbyhd.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gngzocpld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gdjqxcfmh.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjxcanemj.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gndpaatkh.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtggiuoas.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gelhtqjxk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbifhbtpx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gbpduaoan.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gjegjbvzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gdakzgrho.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gxplidkdr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gzeklpznv.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gcktvvtip.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrldwqac.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcwlitvk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gugeompty.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdhsuxzdj.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gklsuasid.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqukzhamk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfmfmrpo.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gkqvfwnac.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/godbhzywv.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdeaeqom.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipndjkap.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsyvsllx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/giemflkde.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gqbujwumj.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcnvhczp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/galqijqgt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gxicfdjvr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdzmwfzq.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwzxjurs.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrsvwkqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaambmoi.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gonkxcyhk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhiovwk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gttfdmqal.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gorniwutv.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gfkhgfspf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/galzrvzfk.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtnquozp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltvuxekp.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gfvrgqcdj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxhczdz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gokysxzut.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/guruncmma.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygjzispx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gretzugqm.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrvkohrd.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gudmnrugx.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/guzrwgvjh.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrbwfozi.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpoqoshqq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gcsqwcosc.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gaijysdni.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gevoiczpr.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcpuphqo.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gybbodpip.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgtboshb.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/glmygdglb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbsdpjjh.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshhrwxsz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyratclm.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gruwktvqu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjkbluef.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvjpdid.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gosparbpo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgxafoft.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvhlvkgx.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gzawkfyup.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbqwzpoc.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gyktrkmiu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmywwyjzh.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjzyszrj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpgmxmuc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwmtkpak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/giszmkdgd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujrjosyg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpuugjzn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxpsbtlq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghnokfitr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gccydcpcp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gillvjuca.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggksrzhpk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/geqzeyvkk.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/ghtbttphu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwoshwgf.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gilbbnhlr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmweleuqd.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gaskimkhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaitwmdk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsarmexxi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/grjusxeal.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpylgwfnr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxcgfbyb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gutxwwlut.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzfmcxne.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/grjrvpoio.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gealjeiij.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyshmksoa.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvpzzbmj.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpbihwzwj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcovsnbq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmjwdiiny.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gcsbkrogw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnmuejer.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gedvoiutc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufyhjhxm.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhydybz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggbeumgqk.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gadgkqcvw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqbxznia.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfodwfvm.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlxgtdof.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxnrqohf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gocnehgks.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujiqvfw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gehcnzlur.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmktqjjhx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gdjarhmah.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdksgtnw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gckbzuufa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwxtcauup.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkwrfeulj.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gdnrmsgxn.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkoosxb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfpxgzzd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/glwydrgvb.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gajanxmcm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gpphlfmdk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gvctqgllr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gvqqumhcn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqbkbsdjx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeowniyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfhoqrd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqscnxcsi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbjpglki.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gvupyrglu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsnxlqf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrhcqkg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/grjbnlymp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmyuvuuv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gziwzssat.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gywujywmv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gqcuejvfc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gnbyutjje.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvddlzqh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdollhhco.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcukceuj.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gcrmoikpq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvecsnaxp.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/grakyjizq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/giehnrlrp.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gncypyxft.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gfyzcdzci.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwqutfdju.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjuvkktth.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gpvonytzh.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzatkscj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbhzrcqa.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsltfqxbc.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfcdqydr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/guuivqvyx.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glhuxzilw.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggcftsuuh.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gefljlbow.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpdjtzdhl.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzwkbzua.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlufpjel.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gceoieika.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtrlwymq.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gtywxyazi.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/guoyivzdf.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gadbihlzj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gethduulg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghumrasqt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gixdgqqzc.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gefuivkps.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gqgzzuwuo.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gomoiltwa.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmueiwung.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgkyvjzd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtssplpii.sHtML


<!-- 参考信息 -->