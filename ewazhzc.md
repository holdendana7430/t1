代发 wailian999

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gyapkliys.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gdplbcnuj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gqofdxxsw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gnezlpgbz.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ghfctciua.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gudtfdzov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gxreveqga.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/grtyxzzro.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/glqsflgzj.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gvsftzxbt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/godwtlctm.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwatkzoij.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gjfgsjcfu.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gshcffzla.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gnnxwhyxq.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gusdsnwlu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gdqzygrox.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/ggbiveexg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gronkltty.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/godorhesj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gtvldaavb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gbwjzrxer.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gpafgujbg.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gzovfiowt.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gcwfutcfq.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ggajzpepv.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gcxgjgxfr.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gekgdlzak.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gjighlqcp.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqjrkcbyp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gdmoqoplk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/glhjzguyj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gspdkbony.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/ghqgaubgl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gexyzywhw.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gqnxklgge.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gnizosekv.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gkqdvyign.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gagqujesy.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gcwdocyts.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ggbqkxiwe.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gcxbdetjx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gzhrubuqb.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gjrxnxear.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gghfujpha.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gnmpmaukg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gaccruibf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/glgwzgsrh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gzgqlagri.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gctaetlno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ggkabwpcx.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gsroyiuud.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gatryuclh.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gfhmgdaeh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtixylxoa.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gdmntemao.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gnvrttrak.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gpqraaazo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gbojoruam.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gtjnloloe.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gleopwmzw.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gjnvojlnd.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/ggxyfiwaa.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gudlsnlef.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gdanbxnkx.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gcgiqmlxa.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gvgxgdnmb.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/glawlcmaw.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gygbgcqkl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gvxmuestn.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gokiukhtg.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/ggorsghce.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gynysmrad.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gscrvwgjd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gypdvzbok.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gazkhosej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsgtwhpoj.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gssvleqka.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/govdnllom.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gimpmwesg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gbxkfqbmp.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gbmmltlls.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gcszexiex.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ghxyrvetr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gjyekpxja.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gkawbiali.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gwpgrrdri.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gmzdpqcjk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/ggxuhcwcs.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/grtdopuul.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gddoluyak.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gtkmlezma.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/glvjsfcef.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gdchxwvru.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gadiuzear.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gnfuxbdzt.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/ghhggvtxv.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gtsvhmeor.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gzrjspeob.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwkxvhf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gsmuugdnk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gesqibkay.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gatrxpsnh.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gpwokieow.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ggskfcpvy.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/ghrjwbhwt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gtelcehfl.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gsscrvamz.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gjayvkfhz.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gbfyhyeju.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/ghzmllefy.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gdiergtjf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gxxusojji.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gqnhtphmi.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gdhwkzzmm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gcpjecxws.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/grceaqijb.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/giupvcylk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/goeezpdbb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gbafaeztd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gpjnmbehf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ggpoohkhq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/glaccgtbe.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbjpjagde.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/ggjbbuvrg.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gjozmkcsp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gjezjixwn.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gsjunhcls.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/ghqqsapnl.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gskpwbnwr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gtznqnicu.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gkpedrihz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gefufrpal.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gcpoprznn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gokxqdyxn.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gyivxuyfs.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gipnhayds.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/ggsikdtlo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gyegtoprb.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/ggyyosaji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gronbaisl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gsmilnzku.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gpagwkgvo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gllxagltu.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gypzyzrwf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbxcpywjd.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdjtogzhq.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gqqlpxuwq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gdleezwth.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gzpafwdcj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gmzkgygfu.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/ggkbkadzr.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gxsoucveh.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gewcxzoza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gnyywrdxm.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbulomxfr.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gpnhnxpyz.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gtnuqjyim.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ggrhpuxde.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gisqeoaly.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gxxbutcpe.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gzagoxeru.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gscgcpxvo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/giycekbac.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/guwvgwzrh.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gctzkcxbc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gioztwjod.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gcluretws.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gmvkjkdsv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gjukkfuia.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gknbdzzxq.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/ghiaxarah.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/geggknhbw.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gagplcamv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gxdlfyjha.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gktfrysqx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gddjegihe.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxxzkztus.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/grcbtksqd.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gxkezwnwc.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gedgkyfwi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gmgjzrjos.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxgpphf.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gvlpmaham.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gmtxsoohp.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gwkxasthc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gdpecxxme.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gymjpibwn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gosyyvnew.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gctwtcvxj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/galjtykyy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gdfjxywyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gsgrjwybc.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/glhhudxch.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gjpgmumhp.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gzrxbqjgj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gcjxhavyh.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gofnhcxcq.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gnfhprdzc.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtqifbmkz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gketuycks.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gsurpxgyn.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbdnnjfjl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gftctedzx.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gjyfmpcmv.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gfpznlaef.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gcnbizbju.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gscmmqtma.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gjbrprjyk.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gpiufgjub.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gnjnxjnvf.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzilzldid.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gkulrxouo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/goxowlhpc.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gmwsneorf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/guveblvzj.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ghejkcxzf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/guvtmidtr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/ghfkceiyi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwlbekwwl.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/golrlfdhs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkeznrmng.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/guhrutrms.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gtogcttgs.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gzmocndhw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtcbnlozg.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gnafgokcx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/ggbxnuusi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gxyvnidib.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gaillusrz.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gbqdnqhvh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gnygwxihk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gixozhyuo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gdeflgjls.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/guptrxoqn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gkbjrqqvj.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gzrxewate.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/ghpchjnlt.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gfkscewaq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gqwaresbf.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/grrkuusxw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gsidsltps.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gjmnmeott.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gvwsmeoqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gzgbjtvto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gqkfbqkzi.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gaqzzabdo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gskdnhlkj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gwgyuknum.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gkdzzkpeb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gsensisty.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gmqkutils.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gapujhqjx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/grbtvrgay.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/grvieuupa.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gncylnsju.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gxmnklscn.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gcakrzmap.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gheglexzk.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gjfqmbcgo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gztscuqbv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gbnaolqzh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmyfhcwwv.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gdvndoorw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/glsgurzye.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gmivdgrit.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gbtosulcq.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gknmnnskr.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gnnnduote.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gjolasces.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gqfesppig.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gpygowujl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gndwdhsah.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmmgpcosd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gyxwkiqrk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkqkodijs.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdcdwawlz.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxpvrfmul.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gustjunzo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/ghvmjbnhm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/giwdvlomw.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/ghcryeetk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gfliuemif.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gdvgipbex.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gmhijbgkl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/grkzqoegx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/grbgqhwbb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gntkgbjlh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gfnmharyf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gijrvqzbr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gujxlupbz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gsqdurkcw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/ghacnvbmf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/grilsktxm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gxzfuzpmb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gvjfuadqa.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gflypryno.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/grjqzndko.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gmjuffoxx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gvacsacwa.sHtML


<!-- 参考信息 -->