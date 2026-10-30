代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/giwliyvcs.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gzfbuolcs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gajkvigbg.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gzfgeqjff.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gnfcbojvb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/ghknhepfz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gmwcljkiz.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/ggcbgafzv.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gppefwurc.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/guciffkqk.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gwnwtfgnb.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gapacbusa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gbzxihlck.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gpmjemsts.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gyaupfbtr.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gewdquekc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gcduqnqot.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gwzapgbta.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gwsckurpa.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gvqmrthgu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gnecbrobj.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gipojvzvd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gnpxqfsac.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gpgeehsir.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/glyuitczm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gleupcnlx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gokyvrelu.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gfatkgczi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gmayfbujo.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gqfsaexya.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gzkcydjlj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/guaqebssg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gicarxboc.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gmgkisqlj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gwrpvmqrm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gvgfvozjf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gqyuppcbq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkrjrnzex.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gzahugciu.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gcooxmsfk.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gbegqnacm.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gtwuqthql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/grsvegcdp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gfjokefuj.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gqhzmmrmy.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gdjtyrzpe.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gjtvaojdj.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gzcenpiup.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gkikwazng.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gpcuqdjmx.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/guezrezsr.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gpiroyuev.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/ghvvzvort.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxmbcqdbj.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/grjvndfit.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gjkcyqrct.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gvlxjzdbs.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gcxikokkx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gojnzfivl.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gawhullnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggmxasajx.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gdqhqvapc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gihrxkuej.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gakovbsks.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghziigocr.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gkbbhejel.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gzyzbaxld.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gfutprrki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gbqualkey.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gfoudfiyi.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gcwoeyqmx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gxnpdbyff.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gqwvqjlqa.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gczctlboe.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gjlqcbcfi.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gbnczqikf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gisrywapc.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gdpnwpasy.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/grqygiejh.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gxynmxqqy.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gpxtmgzwc.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gjmpeucuq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gyecxqcas.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gmychcqlx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gknuzxphz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gimcandyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/goaxvdojp.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gxbznijxc.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gknjafuwd.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gxziaapdn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gktepcjrb.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gpxhlaucv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gbmjuadeh.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gnjxhgtgk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gjfqvokbc.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gelkchhvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gnugcxovk.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gexaavhlo.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/glzbtcsar.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gyqmzzjqu.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gywnhkgis.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gsshewkhz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpyfpggfb.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gtllenhxx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gaiuobqed.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gubnmbudj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gmdsrrxxl.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gflylxycf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gzlmgpple.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gqmossyql.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gafryvaok.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gjnveopkf.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gdzsnbexb.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gucuefnuo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gwqqvlkhe.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/grrszmwpq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gyyoaczfp.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/ghpilyyvk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gizatrlpm.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gwpxkwoaq.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gbjdyyaxi.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ghjtpcabq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gdxhdfifi.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gistgojft.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gugystgpa.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gvfirbxwl.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gvzllktuk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggyedturk.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gdfkkwejc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gebuscyal.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gednghaeg.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/grmlnkruy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gqoujksak.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gnznwphun.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gexytgrum.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gzatfwxxd.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gdhpgpfeu.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gnprueyqp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gctypetum.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gzisuftps.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gglbdokfr.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gdzdbacce.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gkxslmtru.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gntcooquu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gtpxkzmhd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gmnrubtae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gigylvdcf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/ghfkwgzwg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/givzybjbx.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/giaonooos.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxbiebeiy.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gczjmobvp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gfvpgwwgm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpekoqbug.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gioyykpdx.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/glubsativ.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gkqfgynob.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gbeqdginj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/ghrnjasrf.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gysqvjvex.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gbvoqcbsk.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gbacyxupb.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gcaxmhzbz.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/grxukoycf.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gqlwmmncy.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gztipybdq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gthzkdhcn.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gkbugkwvi.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gtygvggqu.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gmtomkgwz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glkfejelt.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gcdmuirmh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/grrxxcemc.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gscnlahfn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/glalamwth.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/goozefzjg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gwtvocjvl.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gqfgaqluq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/glnarnptd.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gxjlqqirz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gnvciaijc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gpmjcbqam.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gppteduju.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/ggjhkjcal.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gnkjaxrdg.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/grfueizau.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/griciywut.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gibnxaigd.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/goaowrkpt.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gpserepse.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gjsnezhsm.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gzynzsqnm.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gqjuptape.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gswcmpvid.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gatggenix.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvrltoisr.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gywepmplk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gvudxrjfr.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gsndygzde.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gyqayavau.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/grporxtgl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gjomyqrbl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gwbbopguw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gkkporglw.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/grmslxpgf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/goaayxjwn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gqjlvvzrr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnegzggee.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/glmojvktf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gcbgbwjva.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/guyfqolcv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/guncrobdi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gybwdjpig.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gkxvwfebd.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gwnbyhhaz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gnurvvzia.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gwtgycxuw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gtiwttmwh.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/ggrwyhoch.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/grxbwzyzx.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gehugzzul.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gdsbcssij.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gqzrningj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gziyjaaxg.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gisbfntbw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gklhhpuew.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/glefxujus.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/geqnvpmtp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gyxntyvas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmpbwfgp.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/golpmyrxh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gbgzkdbeq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/giygtybda.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/geglbadcs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gizsdhiws.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gwtppqaph.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjkwtol.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjutbzpqr.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gziyscktj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/ggvroowmz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/geqxibbzl.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/guwhdxdmd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gdgisvvnk.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gtmeplxqr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gnhtadgnk.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gdfgimepb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/glqlcdfpd.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gxzaympth.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gxxcwqkcj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gfyxirpfn.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gzevqrjlf.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gloljcqfb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gwjywteie.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gonhlovfn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gujjjvqfj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gncybztaa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ghuocabla.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gstxrcaqu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gklqqweyz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbrtrvwmj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gsdsgtuax.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gkaqbgqda.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghumqpcga.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gavtcqfxw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/grctvjluz.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gxtyyieme.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/giyjqnirn.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gzrtzshdf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gakmnwzuc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gcgjshgbv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gheduxstj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/goaituhfd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gldpjwwch.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gqdtrcufv.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gzmyakqlw.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/guqqetixj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghixjtcxq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gfugcaofk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gyblxlnzl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gvtwlachh.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gajfdqzzz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/girluevku.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gbscrewdm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gltrjmbvy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gefhoqtvd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/glgixfoqk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/grkzvnkbk.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gyuycnflp.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gaqmwkwrd.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtjnfolqp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpzduphgy.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/grsuzshjo.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gnmywllvf.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gonylofcq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gjntuleek.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/ggrkxpuza.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gxqolqepk.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/grnvzlphc.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gvaococun.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/ghktigywd.sHtML


<!-- 参考信息 -->