代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdimsurw.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhimhbki.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsqimanag.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gebantsxr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpdfcpklq.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtpyvhzd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gxdtidcok.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gdeltfnnb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/grzbcnbux.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurdokxok.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxkrfdkm.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtfhmgfv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/grnkdowku.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpklmkymi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gjotneehq.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwejuvdhs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcxjgfad.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gazrftdnp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giorbtvfi.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gjrelhkom.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifpxbds.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtnbydno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gyedhculr.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfvvpkdx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gemyrsuor.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrdnfxfw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvwiufcwq.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwtlpbckr.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyksvppga.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnulimdh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjdznfwwa.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqgzfmod.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdreelawd.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxmpdex.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gsddyrmyb.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqbapnul.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvneilnt.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gldrklrmu.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjisqtfnm.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkxhfxm.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbetahys.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gzgeluvcw.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtzjukdv.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gamsdhesz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gxipdiazd.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gyziyhhot.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gpkosrmug.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ganrsjjnb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqmwolyaj.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeujjsjj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyoczrjc.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgkhlxbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gntqrootv.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnxmrsasm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhiqfkc.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gknjustze.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmefloin.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/geyfrsmbf.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glwsbtpzk.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gvpujkwsl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcejhjla.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gupgtnexj.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggonvjggj.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gwompitgf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmefsseoo.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdlzoyz.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkzbzjhq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhbdxrq.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnemkigxt.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoqsbpfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/guupuqbam.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/glmkxnzjz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxhvxwvg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gfwfqqitj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvabgsjcj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzhnxqfk.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvhjbddy.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/galeklvsq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvizfxaeu.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwkcsldm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ghytfmnln.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gaknrmwvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqokxkey.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gfnudmylr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gkgmfpipo.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gllqauuam.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmoeqgetk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gqnrbquxl.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gmedyfxab.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdibcuhys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggvalvsnm.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbxaurhol.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgggrhts.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxlxmewd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gkykydvzr.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxpfvyooh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtqkcont.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gwpmjkhok.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcgbdejno.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gswnndvcn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncarkawf.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwjekmcp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyxnieyl.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunxemmo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gqumniiio.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzosoupij.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmdyzjnu.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmesnoetn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfdaaupb.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gdhyjdvfh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxrqwmccp.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gobxximqk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaizdwxf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gnedijfqs.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/grwdkrkkq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmbpcoxtu.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmnfvrjgj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkcwnhjop.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxknklyr.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkyuvfcq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefkrpmsd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gictxjrxg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gdhmgpvvq.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gruvgugss.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gqwpiaycx.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gvnlenwem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ghnkepvfe.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqevzrvj.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gridiypxt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garbkfnst.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcjcocvb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaussrpsd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gsydqlchs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlktejsf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gvwwalbnu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnmmwhmz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiqrpovu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlhgwmgk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gaubomkpe.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvfhpjcfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmsmwovp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gyrylblzb.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqbnhyfk.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvqxwled.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ginfribfb.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gvxoqjwpv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtghvdphq.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtrazrn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrwfloci.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqippjkf.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/geybaneby.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gorhajzgq.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gewtinoeq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsjtgpauj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/glzgswmfh.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gulelbszb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gegqzvshc.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqpwamdm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gazeifhrh.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgokykny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnflfthu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gpynznddj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gxojkpqzh.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gguqnhjaq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhvkawt.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gxzfsgkqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gluhmbqcr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gneirjimg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqulchlmn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnasatfc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwauowzjf.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gdvxpfuyn.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gesenuffk.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxjqgzbh.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtgxmeuw.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvzunusgn.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcwitusv.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaefbvceq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/grwjtsogy.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdpkmpch.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylipnlq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gyiezllim.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/glqrysuwd.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnqermmh.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoaqfqnw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsefilutb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvkracjl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhgmwiew.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gsllefqvf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmewdyh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gghivtseb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqjyjspxx.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwqnshwh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdojhwka.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcpwogrf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gixufvixu.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gsyyyffqp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvviqylni.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziheyedw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrnlbcic.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfzvstkfb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gsgkhuyfc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmivdvfx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzjsxphe.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwrsrkate.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtssrmujx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/grehzajbp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gbrtyfzvq.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/galigtijb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlbljrfg.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaclakub.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtagdych.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gqndmhkvh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrmgsftg.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkjothwn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaqcpnuuz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfdosjkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwnpwjpue.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdxbydwf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/grpyxzedm.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/geglmuhoj.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gifvvcxjq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxmbypyw.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyolcnbj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaurozhkg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvmshznl.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gimgltwwf.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gbujfcpcq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjpiaqngy.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/giirulqkc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gsfqfoila.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynvadrjx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzcukxecj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbrqsesx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylaqexi.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqxnmpod.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsnvgohim.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gneyrigsw.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwypgycl.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gqenwqgiz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmvltqpb.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gdyoxznqm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkncdadm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gsecovvpd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gmcseuucm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnuxuztra.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gpccppuqu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghrvabvyq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuzelept.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gswmmhcjj.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqwbvcvey.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjikpszw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghdycayoz.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsaylrde.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/ggftagqbb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtvyrxzq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glprdtdnl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gutbhbzig.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gaqwvernz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gryciowcy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihzjfthw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzpgregn.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gbtdqmrat.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzjtbqwr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gupdapmnp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/goficeibi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdukntcnk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ganykwrph.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gjszglvhl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpzptqbo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/girnuewnb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjulamwlp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/giqovtknw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucheypyi.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwazougmx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcbyirux.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/grpunlphv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvemjikrb.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyaftsjsk.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrtmgdfg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzywfcjx.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjkhbbikn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiiucpsi.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfjplivb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gmenpombw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxqazxny.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdamlrmf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrenjgrh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleulkcdm.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gulxcllqu.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gmheuvzhg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gugdykiow.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gstwkkrdx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/geqrlcgkl.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfpfuhr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzzrlgxs.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gvabxngqe.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiclghiq.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gdkmaauqj.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gvqhptums.sHtML


<!-- 参考信息 -->