代发 wailian999

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glpscoxat.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gyfijgkic.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkiveroz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhfylqzx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genijoivi.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocoxavq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gilfwokio.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmahhyya.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/guphirkjh.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvovwjt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfwbusfa.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gekygcjil.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gqtbezrxs.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpskuqsv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzwcmfh.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gevklxixc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvpynfvb.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgofwxxo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnievhpy.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqofzefcb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghdfqvkqq.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gbtkipwqg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gewaftdhw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnwrlwyd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gddbukmps.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/ggztexxmo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwirtvbwc.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/grefnkdiu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrwbtgno.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gowtyjgwj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfeasjnz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjqymyqvm.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsnmcbxv.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnkukkfv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmuaairg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/giosqypph.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gixhnxbfb.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gdbbobjev.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkmrrmpal.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpijxgzc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/glaelaple.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gsietvahp.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvcnpfmml.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/getfqunjf.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gpqnehhhh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnazpjrzz.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnutlbxvf.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjudysxm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gdjuelazo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiihphad.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gybvevqwm.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gemcpbugd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gazqnalei.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gfgplgxsi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuwggcvc.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfmuyhobx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotddnqq.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaplgwhcz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvghvptzz.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/giayqtqfe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gxsbguzsw.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gxhphtbnq.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gakvburui.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdqwzhtb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxzbiiou.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gliunkqoq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfanwqnf.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gcqqfbgde.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gedrypgcy.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeubyoth.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gusdcijbs.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gccodwuvx.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/ghkssfyvw.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giezwjvas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/grphtwyqm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbozrlarh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdvdwvob.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggvroobnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gamnqaoha.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxppfckdq.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gljytjjug.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdlciserd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gytkbjreq.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gwqcgtuim.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/grdihywzv.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbftchrlu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhmjdubb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsrxsydx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gncpvelly.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcrhelkcv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbimtvwb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/genixybyw.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gszevmcxc.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gchbfcyar.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjocwlpnw.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyuzzqjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gdnudrfsu.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gvevxkexl.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gxekwylyu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gcbutduod.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyofiuih.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvtukxhs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyxeactwz.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gbimelcwg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyxlyvhi.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gxuosotvr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkvcwuibg.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvullmiem.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/grgcsbenm.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjmgnugsp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvmdsqurc.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gqqxczzvk.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gjlencuqe.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/glabizvkt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyloxniz.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gfojillon.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzkyvyqru.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gvbucxqjr.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktlagaju.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnwhsgaux.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gmvpiupjr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfcmezkw.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gceewbwuz.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/grhnhbpju.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdltkjhi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvajgow.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gseilkors.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeteilah.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/guilazlfv.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpwtxghq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gizahxgex.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoyncwns.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaliplqp.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqlfntsm.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gxmmuiphq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ggalqwlxw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gnjtyuscq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gszfexjll.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gblfydxau.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gicmxrnvo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gnromvwyb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopqchqti.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/giircayot.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbhmzkgc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpivwyva.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gdveieald.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gsgsvtijb.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqgfpkaw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiqrzwnh.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnibmqxoo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gjjozsotg.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwsiqguy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnqjjomx.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gztnwzvot.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsxqbogd.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqikyytp.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwvhhbej.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlpikcxa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzowxrqbw.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghfqvczkt.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ghvecopbu.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnsvdoot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxzfbql.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjsdyvrz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlekqpwj.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqlhlau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiftnqar.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guabprvtx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/glsjqcbrf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjsunqis.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/grrfwmget.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gifhwzoyd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnshyrjfe.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gssorylzj.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gkpivnelc.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdawsmzgw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxwvrxvm.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grjbxkfqo.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbevaxtgw.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxvuzfnvq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwlvmgf.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpgncvuoq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfojopwzp.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/goftfmlhh.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvixkwif.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gmaryusjh.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gacozcjth.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmfandehq.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpffprh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsirxpzb.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtwkizofo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gdgmjvuio.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipfghplc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxuqilkvp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gikufvkwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gipjugexp.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gkaqkncue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmljalkrj.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gegzzdevo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbssznlgs.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gddpgeqgh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcfbujpio.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtzjbsusz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbvxlnkxx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxswbauh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gexbntosp.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gskkqcsdu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbubwlyd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajbakdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghirdbcxc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbifppnn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiwjzdtq.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gpxmtfbhi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gzzwgitmd.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfgievosl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtrmloamr.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwybuosj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggzynrfrd.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gyyknjdft.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzozsmlbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggreaurnu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozcuczyz.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gafwyqwwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkkgzqip.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxurhwqw.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhhpyxyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnzvoxnk.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gemegrngx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaurdxuw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqrwmyyg.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gridxwcry.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfjhxxxv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glazvagjv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirihomg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpxkwbpy.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxorvhhq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbjbmej.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/galpusgsi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyozhaewf.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqjifay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/guphfwena.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbzyxhhfi.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmylpugrg.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gernpowjv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvbgwplnm.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gkxwzybmj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsqwwvoh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyothejwz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gupheqwwd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrciyybt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gzjadgfld.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjfyuwblw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfqnyfvi.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbvjwidy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeffwaog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwiwppsw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gtflztthp.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gzmjiikyf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqdgerz.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/glfbnkgrp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gpkprlhap.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnmgetsm.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gyzkmrodo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqdohgua.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxappwz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsppzxqdy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gccllzehs.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvsbromh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjmkdirxc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gstewqocw.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqfuizel.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuwytkmk.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkgbxzja.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/giiluuxcl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gcedftcdk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmicbiibp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtqybjel.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgfagumu.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/giarkzglz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvgolveh.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gdeqfdtrr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gupmkrhrs.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gchikchpt.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmjujuh.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/grltuiree.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcluybcro.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqsyblv.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gkyewygzc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gzygclzmp.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffqpgfsn.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gynyelkna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghungvbdx.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gggzxlhwi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvfdmojo.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrnixhif.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlbajwga.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gawnglhgr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqproqkv.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwlounvs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumqlnftu.sHtML


<!-- 参考信息 -->