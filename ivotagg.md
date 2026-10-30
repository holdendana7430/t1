代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuxxuymf.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/guvxzusxh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gmulbprqx.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/giwzkabii.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gteqzkbrj.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwyslgih.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzrqcru.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgxtljxe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaaiewni.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnwutjcc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gfgfraqyz.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gucfmnwev.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gspiqspuw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswbsykfu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggwtlzoqc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjjprztv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/giuoyrkrx.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/guapxiqcn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpulineb.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gqvwqszzc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/guylagbvb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcsuoemav.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gpzdcdquc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/grsutbamt.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosgbvtc.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gzjwkeygq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/glgdohsgw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjrpbwhg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/giwelfrrs.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesuoznyc.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gktbpzenq.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmzjucdk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdnnfherx.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gqpegnhge.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdncxlc.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gngtitwdw.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxffxtwws.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/galejhvmf.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ggnftzrmw.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/ggeuhkmlz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gdzvuulcg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gatkgcqwm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gykeyfquy.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxweepckv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeimeyqy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbtqoonf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqcqoqgl.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfcnornq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gswboqvwt.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghqfekon.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glskcxvai.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqllprbl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqzusiwa.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaqoksvg.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggotnymme.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/goadgnrsg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gucuddraq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gspainqnv.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtvvatrty.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gvtvazkrx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gtewqlnsi.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghsqkgaac.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryklvstn.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gkswebtxo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeukdmhs.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjxjrjja.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqdmtbk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gedxmqnwp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gifkxvhjg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gjrlipusc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/glfimdjiy.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gvivixwpi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxsnpobo.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grshfzwlm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhxsisvi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwferowxj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/ghuglbtgq.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcgspzsdw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrjrhnvo.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/grgzrbbve.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcbgxhqx.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrikvzpc.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gcfaaahuc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdowperj.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gpndodkwt.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghrawslmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaekkunr.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gmpahecsf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gxszkpccu.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gjirngyjk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfzcbkib.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiuvdwkv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gttorgzbg.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxcghal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gskkyuqyq.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhgiwart.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gsolelfnm.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsqdnvti.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjiashnr.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkeytypsi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gpziatxzt.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcllegamf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrtrnua.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfugamozb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfixxwwyy.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gkenhkojw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaziqvyuj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyxahudc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdxuadnh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwukieeek.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbwjvqwh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrlhqnwr.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvonbvs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaudjqqqs.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezehdgvg.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyteaqzcq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gospxgjfg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuqnxpss.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/golbjuqrz.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gbujoluwz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotgtwttj.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbuubiqf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/ghkcmypal.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjytaoym.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptgiepwq.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghzebceyi.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/grdiljsns.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glggdpkbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gkfqebzhu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpditoqj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gpqrhmqlk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gwsznhqix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gwevexvfy.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gtghvzdsx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpiztdyq.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjwoehal.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqsrrqx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gmbojzmda.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedxzglvr.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjmhgbq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniyobbvi.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gkqduynrr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gijubxfzb.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzshyfpog.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgdmnsx.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtdikixbl.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtondknvr.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjjhxjcp.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gbahtoihq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyixcalp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzdpuypm.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gszuxezhe.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gwezdaxtt.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/guvultibs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gesdazrtx.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbnptdae.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzticgqr.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqgyeamwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gmwymgbyw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnccgaze.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbatwawo.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzkclrcd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gstljbhsr.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gjshxiaqi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/ghddfeage.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofglpsw.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzznmparc.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteibljng.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdkmkyor.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gatozxtlq.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtdaezbc.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjggewcjy.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gukgxtlap.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/govocmxjg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpcucxgm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybmjybps.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxozrrdti.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjampqqtl.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gipbkqaqf.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnspgfit.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyvytofr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqqeqdtb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkdllhpu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfilydpm.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gbogmkeax.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluqqoyfb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtwnowby.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gulqvnuwe.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gybvjqfdu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gppwxxjku.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxgisucz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpteijmpr.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbommfnlk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpgzveb.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glnxutmos.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gkdzhjmiw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grsrwpfeg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvtnrlrr.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvrbefwlc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdxreaeyc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnzcvodg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxbzssqz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goqcxiema.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjxfunfm.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gsucmyqju.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gssrsfyqv.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gitzkhxfs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvunpbjq.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/guteucpof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrwlwnw.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqhifqct.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giedbqrkh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gukgozzkd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlftosuo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghmonrkgw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gmhrzfacw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glhmqxyve.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gelqhqinn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtplbhols.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gelpiljbn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gujwlveyu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyasqmbef.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gigemopmn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gyjefdvso.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glwrbfiya.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gtxgvxgwy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gybxwmips.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjeilpklo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtadwsvj.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gamiqtoow.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjpcxdcz.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmhnjljt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/glzlznoqv.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gucnjbpbo.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/glznbvwpy.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ghuldwrcg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsiezczb.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gullybexp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/globysviu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggptvafqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gjufcxnxp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grdxhzbve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gzwousgpc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpwhauvpp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghivuzvmm.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqimewysc.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrmgalvp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbopeac.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsebnybru.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxayfovjs.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgaorae.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/grbmyxvsw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjjrrnuzn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsudidmf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqgjmpcy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdejdbdk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxisrfkl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gieeuxsum.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gfykobamh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxeonmsf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxzqbtimi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/grvyrwiwz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gloawfbcr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gutkstbqf.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gpeguedfu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gucboqwtf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnpqtmog.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcvrkdiok.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgdwwdfh.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhaxhzab.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrijsajm.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gyfzhpexx.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkkpkljo.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaslrkoux.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpuqydglu.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbedxibbx.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gcmjyzmxu.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmganuxcd.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gyoohvrsb.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbbqping.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gnruhvubz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcyxopa.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsazxrejc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gznkyaerz.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdebzkysr.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gkqiehjwi.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqijjuf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaadksuu.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyertimze.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvcknirxj.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/ghbuiinat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggerwoqhd.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gdkxirqkm.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpuhkxjw.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtozwphy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtljjcioo.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gocxvdrhs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpxiplxy.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grkxnnqfi.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcmtujgy.sHtML


<!-- 参考信息 -->