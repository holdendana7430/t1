代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gskwoudks.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvjlkoay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpngapote.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/govyfvgyh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsekvxec.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpooznrpc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzpobic.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrunxhgf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gwprztuzd.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbsduyaz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gazcpizpo.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbpcuef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpdujein.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gjdbuhkag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gppwlbewn.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbkycqyh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grwjyliba.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gjbctpzoq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gryiljigx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxjqvzct.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gvvughwyr.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/guixdgulw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ghhohlkpy.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gdozywywj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhzydjvn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkjpwkfn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gpsgkijsj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyvzncjrn.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzmqkmcca.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgopkyvk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gionpsfsv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gubpxufro.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gptgwvvmb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhkckrgy.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gocjsgxko.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkcmqypa.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgktsfau.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gibgrfcfq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcqovfesy.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxyojfdz.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyzqlvkq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwycqxrz.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpchgqjaq.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvatmvnl.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gmacscdgz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgkykbbu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhygwkiv.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaxxfrcx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjeraqbh.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdujvsglf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/givtbmtuq.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppviwing.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlxrddhj.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeyfrofm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtmwabeck.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwrzwvbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gdlhtzlzx.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gevzrazdf.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/govqruzyo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuymwiok.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksmkenxq.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlefjabn.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjfcgibud.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwjhvkrb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ggpvsxnuw.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gggyubztp.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcgoeqbg.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/glwylsovv.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/glonzkcvb.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcculaohu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gordxmzfu.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guefoqxmr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gzuvxandx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gtiufhgys.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkowvzupy.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwpphdnou.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkojfmiic.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzuicnrir.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gsjkqiyby.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxcopqsq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbbzjna.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gmjxmwoeo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfimmftj.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqnjoeqa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvptuabqa.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gekbssvhf.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmxlkzfqf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzfedidb.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gshkaypsh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdtfjtwf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glngqjljy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjoqmlkq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkuzsjom.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grefzlbyo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gdvhqgvki.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ghovsjico.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gsocizxrr.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gakpiovjt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuyjflsb.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghisrkmdq.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gmrjqxsfp.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gmiyixzbi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwrvdxr.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzpkdpdwt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gxplxjxgf.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdycalxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuqofzyn.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwpnhocfm.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjznaeunh.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimcrrfj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gteuwdyix.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gpckrwawa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfrhafnfz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyudfxtfs.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gskpbpaha.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gijpahvli.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gngobpjlf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdvzgxte.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegtbixtm.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsohfgvty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/glcowdaxy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkpglexe.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gzikvfysq.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/glcllhqoh.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gatzjliay.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyhhlqpp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbpggfrc.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/grngluoew.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guapxsqxi.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnrqkpzih.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgihijna.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gnvesjdfg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ghitznign.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhttlck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/grmeukpcc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpszqcdk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gpnajbyhb.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvypnoqrm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gyiltbsbz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyekvwul.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gfpeevkfr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqeyujlxw.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbrczgsz.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggtoafddr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gasxswizz.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoinlfkw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gqyhzwujb.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gjircjziq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvnbfrsv.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrvjqppk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhxusgg.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gkutfupim.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyntddlvz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxierxd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsorhjhf.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkiolqnau.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwecyyori.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grerhfpna.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccojlhzm.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyoorhee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsjtioak.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/grizwfimd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqodpemxk.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumqkekr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmcvpqlob.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gztnwefom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/goyesvdcc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoxzmfpr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmwlwhh.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdlhjjsjq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxyvrkwl.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyemvdwi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzslubczs.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjtoyzas.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubmuiwfy.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glixfrldo.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxziwmicj.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpgpujhw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gafjbpeox.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gjldoryex.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvvxein.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcliullw.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gainnvcng.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmnltyvpm.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbxaeqgw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcbgobna.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggdtucudz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gafmmuvek.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxhvulxg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gglhwlxwu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsyknujz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjewnmss.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknrfmgbx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkirvcafz.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwufroebl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvyyikaqz.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gpbqqjine.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/guwhlkslv.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gulyzrbzr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchxbgjvw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gncxkkmjk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gcyzaqbjg.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdufxbbnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwtnxrbqa.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gevkimpmh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gasjurngp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gckdctwdx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaxpuzza.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkifkcvf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwzruqyd.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbwmvmpj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipxxvdvz.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmpnktom.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyplpnwrr.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggcpbxksm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gklwzedex.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gykbmvlwl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdwcgkmq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwzlqfyb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzodkjbr.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gernkoptn.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyftdodpf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gttrhtfrb.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gixwqhvqe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgzmpaxh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gukuixjeh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gicpoqjqn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gbuqfpfbl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghepzfxqs.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gjrfsvfid.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gddnjbrwe.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcafcyikv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsjnpdgdh.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gjlthqaeh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gapgmqpan.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/goowkgiza.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geedzswib.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gdhbkptdq.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfrmhcacp.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gyczicrem.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzikihmh.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gcokhqdij.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvhsvxqo.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gnhiggcul.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjdwqrddz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwhijdwtt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvicyvya.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gprgdvzyf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geemuezef.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrrcdahd.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geblocglk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqbgakhk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gziddbqyn.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqymhew.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gyeubakiq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gexkzkrma.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysqyseti.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmzrxmiu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gurbyiiyv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowqrbudz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gupjhgcyv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grsfhaszb.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gwayrketw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhdeztax.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gseevuybi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gplfxohfk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gecwbsyhj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbztsnnf.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gswffnccv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giruqfkvj.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gbniormkl.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/guwlprdhh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gucbfgvrm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gygfffzim.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsunrdvnx.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipwfarff.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/guscfxkuh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiesuukq.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyozujnsw.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhqiahhu.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwitdoxhp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcboetnyx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmqmbcdl.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtulnkukt.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjjlmiu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeomvflt.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gtuqdsnqd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlczmvyy.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gddigrmnn.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmanbrjh.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxsxdnxx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/guskhltco.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtagquon.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gqchesaqk.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gemhzmoys.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwrifcga.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjocsptz.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gyypkzqai.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gfehrgqis.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbpkrgwk.sHtML


<!-- 参考信息 -->