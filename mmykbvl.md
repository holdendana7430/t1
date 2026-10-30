代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gprvxsnrx.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gyunigmmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gdhgtrxdw.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/ghlgjkiqx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gjmbbeffl.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/ggsaqtmuh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gbciqnwog.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gnbgjulhm.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gqugswlkv.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gevgutpck.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gjodpfbmu.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gwyaxtgps.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/ggjrgrzen.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gbntpuvqp.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ghdwxvwpt.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gjtjjessw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gjuyuteoe.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gtkmtrimy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gotynpvbk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/glkslkrrr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gradfrkyd.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gynvdyzxc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gzzosbsxg.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gwnvmmujd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gvjmzzgce.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gyqhemqhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gnvbitjop.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gxwhsafrp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gnhlhyqnl.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gwpslmocz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gwrzezanz.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/giijzrefe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/geyphsvgb.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gifogcedf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/geuawosnv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/geowzgumt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gniqzrjcb.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/ghvciguya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gdhxrgjpl.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gmqjezfcp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gqthahrdz.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gbzjeykzu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gqtteoydu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gbmaiafij.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gfotggbie.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/graawrskd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gyymwgltr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gttxhufza.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzlwmpwaa.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gcikamimn.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gkucdqedg.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gizgxbzem.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/guizrenxg.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/grdcjkbwm.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/golirsydk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gvijwostm.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gntcuxmhn.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/ghdirsvcb.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gsgrqztul.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gzervwmtu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gevkzwxdp.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gywbfechq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gsrcniobs.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gwrwwvqrd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvlstxtae.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gpqlqoewq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gtjegehev.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gpmacrxcg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gavtcsijc.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gkroyqapw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfzjlrzdv.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/grdoojrjf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gajqelhgu.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gjwuzhghg.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gobsohwpj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gwkigmboq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gvwpxcdox.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gztdlsmhq.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gyxybjsdl.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gsoyqweue.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/guvtgqtqp.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gtosnrcco.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/ghiztkbpv.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gmyfrumiq.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gwqhfeoyl.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gvjndoqlb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gboezzmmb.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gmhvjvovm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gnpbfhvae.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gseerboln.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gaamumeus.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gqxrtkvhr.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gituyafqz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/grvzghpin.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/grnuuztgw.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gxxpqlzhd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gtnxkcjeu.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gmzhybfqb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gpzpnirat.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/ghzzevtsh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/glzpuxpzy.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gvqvzgzms.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gddynrwqf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gywbvrlmo.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gifqdaaug.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gtukhedwc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gitnbxlhy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gjaeroucd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gvmyxdlgv.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gdiyamoqk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gnyuaqltr.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gdouhcurg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gqidltvbv.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/glvemwrbq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjnbvxfnd.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gotlyaceg.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gouhejxru.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gkomdudja.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghxhbtswu.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gvndbrssn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gdzkfmaux.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gyrmptqtb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gvqdmcuqt.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gcyswbbhz.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gmekeznge.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gwdlywfbr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gxxwmhjpw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gvveerrrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gqyfvdvls.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gjkrkztgx.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/greiikfbq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glfpzhtct.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/giblnepjp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcedncabh.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjysxuuwt.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/glzadfjcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/grtdcqvjq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/guxyaqelt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gxhmzejtc.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gtuxuzrqn.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gkpcdukgd.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gcjufmium.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gpoqwijlk.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/ghvofykne.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gnqtqmelk.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gokqrgiyi.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gxyzaxwty.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gpdthlxlr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gcxcheerd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gbowkwugn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gzqvdeila.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gjdltayjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gjdujkxch.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gyobwrkta.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gopndiudi.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gywaajkon.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/ghnxygzgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gnnagcvga.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/godtkqlqw.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gjjemzqwt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gxtfhrgvk.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gzzygjkip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/goiqcghfj.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gdjjznkki.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gwbvrtfjr.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gwpnmgjps.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gdjsqaotd.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gawfeuuuk.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gwsacqzui.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gocjvomyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gettfrhop.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gffovmtsy.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwtakgaag.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gnnegdiho.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gfsjftzzu.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gelwjtimb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gqhrabcvd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gvgkpaqzx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/givvajxvk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gioujzlnd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gcjweqlxc.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gbmwgrwww.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gvuovujmg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gqivgszhl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/geayzieui.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gtraonmkc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/glpzhaylq.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gcayuqqvi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkvuytdd.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gzzxvxxqf.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gimgsbcyk.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gqhdblldk.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/goilcnlfd.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gpjyqdvvh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gbgrgcpfj.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gwcnfrcmn.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/giuwwwlcd.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gipqocoji.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gobxuxpbx.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtslogbzu.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gmoitepuj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gufecgpgj.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gqpjamwsg.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gekapczus.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gfcfiaoyx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gkxlimivu.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/ghhqgsoqv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gzkdpowbs.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gvqdhkbtk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghdqlcriy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gwckaaoni.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gwnwqwvxx.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gipdwwdmf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gwmwsthux.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gxnqngdsq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gtkppxtgi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/ghfhdpojd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/geidfcggz.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gqegdoaas.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwoquotrf.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gvhnzqxno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gtrgrtoll.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gvfmddsfc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gvnncpwyo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gcotbpwmy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/ghloowfht.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gosepbqno.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gjduicpix.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gzyulxzve.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/guuabdecs.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gxbdydgzy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gobwednsd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gmzroeiie.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gvevotxhg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guvaffali.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gezrqysfx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/glglrzzvo.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gdbonxieh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gwothrnxt.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gdmgblvck.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpvkmzrcg.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gpbqykpyz.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gkjllleud.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/giqlwvfjb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gxzuwwnmp.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/guutrkvqx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gqvhklpnk.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gndfqzwaa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gdgjqakso.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/ghvxtfyai.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gxvalumzj.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gvmjsnfaz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gzwohbtpq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gmozmyejs.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/grhknmket.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/grehfswwo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/ganlqsyem.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gahsratdo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gufssxzzk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gixpjiaky.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gnbxlpssr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtyixavzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gjagqjrsu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grdbbshoi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmiocckcc.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/godenswot.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gcykmhgkd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gxetbnmvm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gnjofzrfg.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gbviadksz.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gjsvkcjha.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gfhkedhoi.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/guntuelun.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/ggdgnypoh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gfgdftkrj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gomhrzjfs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/grjjjcqip.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gshzinenw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/ghtnamvqm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gjivqybmb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gyrzenyca.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gvpvmqepc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gyynuxdgs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gjqaotzgv.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gbjfwjffo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gougnlssx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gapzefpzd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfmpaqnvv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gxznohezt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gjdbxbyow.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gvddwfell.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gnqvhgpfi.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gxpibecdr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gyoekbwto.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gregspqxa.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqcnepeav.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gycnsziot.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gjttvbufq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gklehlasx.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/giuyfkrpo.sHtML


<!-- 参考信息 -->