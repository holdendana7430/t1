代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gebefkvfb.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gigptnmcd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gddlmxcur.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzotuhl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/ghzapwwjr.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gqmysprlw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gjapkilgj.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvspckjrh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkjxcbvf.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gulzoljsh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gptqtxuov.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gliohkpsd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwbpljrb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvfprpon.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtdpjrmh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuvxqrwl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrhzvhhw.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gyvkvpqhs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfswgiyfb.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gxevtcblu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gietdrxsw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbpdgza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gceqpqyjm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplykpckk.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhpzmdag.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjrbtjiws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/guovcerav.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdatenx.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gyhruzzgn.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/geyfmqdcz.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdolptxn.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhiwrnv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrsmjdil.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/grgbtgzbl.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gysgodqwh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpfolwru.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gofzqjdpf.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqmyifezw.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxxabkap.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ghdjzzmgy.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbknvfmj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozjkincm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gylzfjqbf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgiilju.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geiekesid.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtzyppna.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/givnluorv.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphlgceyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmkbvjce.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/grbkgcmkv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhjrnbcm.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gnmuqbtia.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqtapcovu.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gssvxsfyi.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsftikvl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzxpgmca.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grkzvkjjo.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gibagpssp.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvxlqeqb.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/giwneodaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqxzgwgs.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspycfavh.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxzwdbyj.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gbqisfzob.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicqhttvo.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdkiivpch.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gctjomevr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqsadmmg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gdzmhabqv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geswfbjsu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/guprmxrdl.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/giasfevez.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyzgpplo.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcymrkqqw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/golyjrbbo.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhnitjqh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gmernevkk.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/guoomirqh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaeuqxfa.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gsrstngne.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gwgesaiju.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gizumuuaw.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmlksnjsb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gvetqzkox.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtfzjdsr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmnppjyl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmulxkzjw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimqwoqnt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtbgwlys.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ggguoequc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcwbjzcw.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqztekfal.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/guwiqleam.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/goikykudi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gthzdxjcg.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxafeysl.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gbytdxdqi.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goykaquun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkhwmubkw.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkvtrafyi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkosozgb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchusmqzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gikphlwws.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdxbjxiu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/goftirlsw.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gsxgamoni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcxjqqlwb.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gkqimromy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ganxpobql.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gqrvfwypr.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gshvfbony.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glchtatwm.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gotylssth.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrdtpnla.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givyecpjp.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gqorenuwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehsnihch.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnukmnux.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzimkzach.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gdxmcvlxt.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhtofgy.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gvsogdbvk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhpogkr.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfitzgbo.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/geumkbtve.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjekcshvd.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gyxmsgasx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkawgbmp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdykkqcje.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwguyalu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnsnqxg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepbbjrny.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgrjnbs.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gvryituzf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdfmhqgc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteyhifry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gbkrfjjpy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/giegiozwt.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtlukiiv.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbsdhcqep.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdrilgbl.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gsqxdbigs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gjyscrbhs.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqftyvq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrwhxmjc.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrbdewsq.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqxeiiciu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjglgyla.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmpglba.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/glhqulfdd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavqtqaey.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteznaarz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgijllqp.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsrremkq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gukrsfbgd.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ghjcgxadz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmihhaugl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcazgucq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjpxkumn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiyixzxt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gorvpjmrd.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmlxofvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwufpvucf.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtjzubwuz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqxoyikj.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfweoiqga.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcrczvxi.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwlyadky.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkoixjbw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqgtqgrx.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcipigntc.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdslunkfz.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxdniwnr.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gahafyltg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/guynhmjyy.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gwijmthyh.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsmypzya.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnvypzie.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ghtshvhza.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgzngrth.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzuylxtm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqhqqpxr.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscdiypzv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gydqftkiy.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzncqgkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfhrrhy.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gwywetqrh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvwrrwu.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfzlhxpw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdmwnwvv.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/giwzkxoht.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgxwbwox.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvfshazb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpubmctvh.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjkrpkwtc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsxmctdb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvvbvrbh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaojadky.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbhpyflpu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gretlzriy.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gekzinsux.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwphavndw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/geqltmgzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpazqhjgc.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdqecxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gkbtdivrq.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoetrupl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqnfuiuyt.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqrnheie.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvpzfnbwr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdftbeyk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgeoneof.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpamdsgg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giqjayxwx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gepzsoteu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gltsrlokw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/geriwknak.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyrkjslh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuzyrrts.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/geebayrci.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnpadzon.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbmurrzh.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gllsctqem.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gtlmuvnow.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtrhktqf.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gkcmszdut.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkkwjqzc.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrfheyfv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmpsiseju.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvifzuqf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gyxungaqw.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gteqxmubi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwxrzbtr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvndddyp.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gyskmfggk.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ggeesrgao.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqnvwmhh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjyrcngp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gypckmkzv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggetsajlb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gukmptxjb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geucupspw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcmhqdry.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ginozbxoh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gocvecprt.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzffhpwff.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjygzjnsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzgmvtfm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtsgvgal.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gquhgdwtp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvfcvxey.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqrduirg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gskkqutic.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gchftfvda.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/geyacpubb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpltgkhj.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgvypikg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gpwglynvi.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gaikfyypn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhauusdn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqozkefva.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhbcyzmd.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzmbavme.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhxgjifp.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gaqrkapno.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/grchkqeqs.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gqrybumml.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpgxmqtg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlvupqmd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqdwnmoq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxgicpdw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofmusegm.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhtrkre.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfysjfpa.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmssdwiap.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchjupyxo.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gkowtltyj.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrnogiyi.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gyiilykut.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/glbynwxkl.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gfufthzun.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gokpftzov.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gdvzppdfr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/grgoqmtrs.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwclhtayr.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvtwzkvu.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyaurpra.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gatzxpmnr.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzdekfdjq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqgjueox.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlzuhwsa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksswxxtu.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvkrfqae.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gahpvresh.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gukojosfc.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gspbtlcgg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grakijaok.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghakgehyb.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gcivjddgc.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaizdedi.sHtML


<!-- 参考信息 -->