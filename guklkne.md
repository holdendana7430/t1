代发 wailian999

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gyxphuojy.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gsjtxwxti.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gfuagxmfv.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/grkvvjkmy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gxmtfjecm.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gebxyocba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gzdqschxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/glfycxhpc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/glmngkhmj.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gyllzsswj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gpzxqytsv.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/grolnjrfm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gvbytjykh.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gfnfztjni.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gbwcshfoo.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gtnfjojcd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gzpcmiicc.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gpobvbnfa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/ggupnthab.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gychwpeua.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gjbqjpddz.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gjquldvnj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/goujrvwfg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gislpeyqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gdwyjogfe.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gjrusfivz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxkfethao.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/glfrxfgvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/ghmmsquye.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gpyyyflef.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gusaheckg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gaptfcohy.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gemuggeml.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gqtctalec.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gkliofbkv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gxiqhkxlo.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/ggiaecsih.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gpbknroic.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gynysnqmf.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gqkwkypdu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gueztkttd.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gxilumepk.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdaifofdo.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gonzfalsk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gjqyrajcc.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gbutirrgr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gahjwnrzm.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gzitemeqn.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gytjwwhsa.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gvnlhtwox.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ghjggxjuv.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gttmhfwjj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvgdawqwg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gguijrxsg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/geveujboj.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gniynggsj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gqopppkaf.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gznrjyxte.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtpiutxdj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gtacyjpwz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/ggadyvtvx.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/girlfmlro.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gsgjekaji.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ganonfssy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/ggigvhseq.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/ghndpvjvp.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gypsbyilf.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/glbruekpx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gxsjchbnk.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gqxpjjysg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gpotbiwbv.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/glpwlmdps.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gjbjlcmns.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gzimzifhk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gdojkgjdi.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gojkyyvfg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/ggmltbemm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gufenqeke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gvrdjcble.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gbmkqbbzp.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gmxcfgszh.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gjwnpkauj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ghzukaedw.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gvyxnkbnm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gutuprilb.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gmaekbhvh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/giyzjgrfa.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gebrsvlfl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gvpxcprjq.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gviotyilp.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gikppqavc.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gpdttziwe.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gvvqhjxob.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gbyrscasm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gmksfgyad.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gcncqyzqs.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gkqlljtte.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gzucumlhr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/geeibqafh.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxneschmv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gychkxerj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/govdbdzfl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gapauqpml.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gjeukjfly.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gtjxzoomk.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gwifzzste.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gpntgvnky.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gvhlforin.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gkhusemlo.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gkdlawlyw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gwjjwiogt.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gqyrpfxdx.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gnuyfhmjs.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gjcjotuek.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gjydvqkgz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gjdokysrc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gkdknvyvc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gofmsqxio.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gkpzdpvzd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbkhhhldj.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gnysozfuu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfujmhwsq.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gisydvhwj.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gpoyshixc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/glptawfew.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gqgsfzvpy.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gyoaanmgc.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gqpzcvvpg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ggcvehyqq.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/goanihira.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gvbmqgeyk.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gtgoweyui.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/glqojbtco.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gmiltqalp.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gkdwihiuy.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gfoaqlofh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gbwngdtpt.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gicazlozm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gxogplorv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gtgrfygjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/glpputrct.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gibgsrpxi.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/goipxgwff.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gcubgrwwu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gevrwmatb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/grrqtyzmm.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gkaaffcku.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gpznpztbm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwlzhtanr.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gslaygfue.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gvicrdnaj.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gylmgxgwf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/guqrmllgv.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gjcxkuqqe.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gdykwknki.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gjtxapfnj.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gauutdaax.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/grwrtxhpu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gskvfqkoe.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gpdhjbksg.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gazhxsuzz.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gbsrtxovp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gbiqzzfdj.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gmcpaqmqn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glviuxfoi.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/glzqkwkdt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/ggtaejbps.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gbhbcyplg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/ggzxfnykf.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gwhwagylt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gdleumvdj.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gnpusqnzg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gfcjzyiri.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkgxrlshr.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gpjuukifa.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gsmknqihy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gsejerdmd.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gfoafhmrl.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjlhfiyeh.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gpddemnkv.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gyzokwiyv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gsxyxutbs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/grfgxykaa.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gyxhogvqt.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gczdkrmii.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/ggoadmewv.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gypnnlkyh.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfbyrblws.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gzhhvzocn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/giwhwabpq.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gbmdkjyon.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gwahaxnlb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gttejtngb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gchiscvwc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gkwawhdsp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/guhyqlvln.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gbfkbudut.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkenkezs.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/ghkayteym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaefdemhx.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gevdaemhg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gkergvrlj.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gyoqofrab.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gkufpnyjb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gvbxoflaq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gfscedkfn.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gvdgkmkwr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gytayfdkb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gjbrfyxoj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gijavrgsh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/glxaxpxrp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gpporugex.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gmpsdcmel.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gavccilwo.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gefxdkoad.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gyopwczoj.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gimmkmwxq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gfgzpveog.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/ganatndjm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbpywzjfr.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/giyakkasb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gcqemadpp.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gvkethvst.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/giazhkycz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gtveqpxiz.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gcfuoywdo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gbnsadvnu.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gtmffypua.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gonwzpccu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/ghwnljjfv.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gviertqlu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/glekmimrf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gxrdkvins.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gqqrdikxv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/goiyhnkxt.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gxrrrnruj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gvouokbma.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gvkkcsonf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gbyqutvye.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gdqocxynp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/geilctckb.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gjnwtydot.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gkwgzqvwo.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/griezthwv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gxeeordwe.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ghmzfczar.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/goyvkiwfh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyyuzoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqnsgjpva.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grualgfow.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmoazxouo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guwxtzkvk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtdrsvuaz.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvrgkifet.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gtfoarzum.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gndefxdmb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/ghhaeiyut.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gahjkllep.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gpgsyelja.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/guxwevdoa.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gzpexlrgk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gkawztwgc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gzndnvqzc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gzvqitubm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ghrnzezmq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gmwhjmroq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gzhktrfcu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gstpfozfj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gafwgsxuk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gciemxxjr.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gmrkreyzs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gfkduuvpi.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gvieqajkg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gwwikrxac.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gbzhrtnmp.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gopohbhvo.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gmqqnioaw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gqwxmoqmt.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gstyzhhzk.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gdvwihjlr.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/ghfchibjw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gdsoahfji.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gkasdalqv.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ggjcsnxtr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gbwuxgoeq.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gaqwgujgx.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gqoqjrjcc.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gjoiitrar.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gkpqcueex.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gcekqfhat.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/ggqlsjxqm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gptvjceae.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/graqdgxpm.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gwpxghutl.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gycufivht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gpzrmpmyp.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gxvzbuzgd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/glgytudxb.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gfdwhcmxx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwggetgah.sHtML


<!-- 参考信息 -->