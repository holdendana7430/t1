代发 wailian999

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gylunwjcc.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/guzdabuzl.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gzaimcddq.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gkdhhggfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gzsumclsg.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gghygadkc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gqlsnbgji.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gdjhyvmcw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/grlkibncl.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gkaepxsgx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gbcdqybut.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gcdtbcbiz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gpgimxknx.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gjuonxzmv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gltlxkkua.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gflajqqcs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gyrmwdluc.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gwabvcmdf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/glkwafefb.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gyefujbfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gnlylinwp.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gbuyeklsf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gzsyeejgd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gdxkjbqrv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gminyjzhm.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gllnkyyun.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/ggxxydlcz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/ghonsyaih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/glgghrgaf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/ginyxeoga.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gctxeqkux.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gxfcvdsoo.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gtakhvffg.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gzmpmyguy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/ghbgsovio.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gtmohzhyg.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gggcejiqq.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gdehcgbnn.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gjgfgchwr.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gsunivxdk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gzvxbrksa.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gbikvywxo.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gedooucek.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gmtpmjjdc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gjtqpdgbr.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gkziqzxee.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gmxftsznv.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwqiurlzt.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gqldlbygw.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gxcxkwpux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gmgakimag.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gkuqzfszr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/giamjowda.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/ggzunddzj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/garpwmokm.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gnrqwarcw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gsirtjbzr.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gxlsftkoe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gltsfynwe.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gamotidod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/ggbtppnqp.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gkatyodje.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gistmmvgg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gvkrsmymt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gmyqgtxal.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gkotlpjwt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfyrwxxjk.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gmphwbsbt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gefizocbc.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gafrbrtya.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gtdswffrf.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gergharmu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gqippwqpq.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/glerfdnqc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/goqkdjzuv.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gzlxhefyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gcuimrbch.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gmjjknmot.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/grpbchems.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ggkethiuc.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gbzcvctnj.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ggsjgfawb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gqcqsrtwe.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gacfiwckk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gqezvgvai.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gyvkypoqm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gpfxphtkt.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/guznessaa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gpfiilhff.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gouzenydx.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gygsasjtc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gxutqfsnf.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gcghryaby.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gupoqzdss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gdnrbphjz.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gtwvnjcan.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/glzgwbgdw.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gnsnaryfx.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gdbtcihgb.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gehkhqjsa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gfdwstgxi.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gfqglgack.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzogypdkt.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gxpivuihv.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gervijovl.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gpndhgwki.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gortrbmga.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/geqmpvykd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gxaufxvxk.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/ghhktjcxl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ggrkceagj.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gukxidtkx.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/ggjxhngpr.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ghrlemyiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/guljjdcix.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gzcmdbzwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gekkutwdu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gpywbfvmf.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/grzrhdjrq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdgxskeyg.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/ghfuymoys.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwyqteggl.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gkwbmcwmr.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gagcetsoo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gvnwqzidt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gakrpoucp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gcbweetiu.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gcwxhqdlf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gmvxntxhm.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gndbgsypv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gluabwclc.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gpbvmfibj.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gsohahdzl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwohvazsr.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gycnddvyv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gtohozrai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gbbyfflnb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/galgyrqjf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gdkhkhrwe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gmnxmmxdj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gqamfjnwo.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gcsvcazio.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/grddkpaif.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gylcntjpo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/glazlmpyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwqrhipyd.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gwjmmxrsz.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbjkokkhw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/ggzumtqpj.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gvkofqyzv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gnldgzmwt.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gyjsgyotw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gpgkcpmts.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gbpiyqstg.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gjsoffmun.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gdtuizeum.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghvnygekv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/glatrmmoy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/givwjybmp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gnntepkis.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gweesfxcg.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gcwlbyltm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gjgaidqgw.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gmekknnfk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gitidmeae.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/grvxapukl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gudutswve.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/genmeofub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gaavfbgok.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gfihwgsgx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/glifcvphh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gndcmlmwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gjukfdbyf.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gijdfyfbu.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/guoeshbyj.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/grhgurfvp.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gdgaqlibj.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gisbjwgtn.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gawexndhz.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/grfjpniqi.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/glwjmttqd.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gdoajajau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/ghtatvtim.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gipiwcetg.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/glsbihser.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gvdxdodhx.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/ggdapqzle.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwqxytfhg.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/glxlmximb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gssuxbtuy.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/geafnbccz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gbjidjldz.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gqfocieee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gadvxhdej.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gwgnqkblh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhcxhvk.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gxjkaokle.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gwxwjjppl.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gngaamwcu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/grjcvbzpc.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/guwxrxfxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gdkxalqhl.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gzrevzong.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/geblisylr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gefbaglfd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gvkvyrzgu.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gqvhmdfzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gdoipidyq.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/ggturjuri.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gfkqyxrke.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/guiboraov.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gqyinsyda.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gmwgbvpya.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gkqokuqgb.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gerpaugvc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbnexypmc.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/grtciuvah.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/grilvikpx.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gnuqbuesu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/govxinaoz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/givovhybs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigvxnthr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwiiaepmb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gxdeugusc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/giwlxxrcc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gsnqjnzwa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/giqlpzfjt.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gayeqattj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gikxbckqc.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gdcdqwlhn.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gpfbixlsw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/grcraxtlj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/glejqxjoh.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gklrcecif.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gstzqyatg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxvkkkj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gpqgvzxgo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gpmdprcxu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gtxnthxiu.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gpfhzcwwj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagjabkdx.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/giagyysaa.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gxaipvqsr.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gtrfkhimd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/glaojcclj.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gnrwdnlia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gjtpdgxvj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gkxzitcpu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gotepzoyl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gffvaolph.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gqoohvpwn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfmutawkz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gglnyjuep.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gpepuloiw.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gdvdliwyp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gzbyurlrn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gxlbttpnb.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gvagaefbn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gtzrazpnc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gngxiimrf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gqddszsng.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gcfefjyiw.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gpaknsopy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gkjdqoysm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxticgucv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gzejwdddy.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gsnbyscrl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gldzmwcka.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/grsrndosu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ggtampjan.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/grpgwchtf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gwncxbyzs.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gheztbpum.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gebkjnksa.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gecwbfctb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gmkcuqomx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gbmlksusl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gnjwbecah.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwwkyiyym.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdtfrtpmt.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gckckgwhx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gzwlvdejo.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjvpzkcfe.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gwudndtul.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gvqutzsbu.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/glxltdjgn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/glfqkilkw.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gvgugvnhh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gcnkjuunf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggedzlqua.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gawchqbom.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gzssckifh.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gaczydbpa.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gwwibgquq.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gyohhpnqi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/ggidbcxgp.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gtsgbgijy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gzbpocadq.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gmegtyuys.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gumqqehqj.sHtML


<!-- 参考信息 -->