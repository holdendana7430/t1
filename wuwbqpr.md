代发 wailian999

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gbsjzmbye.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gxgqklixj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gyhbnffzn.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gqiieueiq.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gnhaniscr.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gewpsmjwn.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gegpzqjne.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gjnscwbit.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/ghhdmozdo.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gpczmnshk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gmgcvakkz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gmbkrrler.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gvrztvksv.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gvgmpmjdm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gcwhhfrpk.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gfzejchzh.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gilutbzav.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/giyrmeqze.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gpcecycfs.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gveqekwxb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gbcuotdfn.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gvqcbcqqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/ggxzplldi.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/giidaybgr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gkgqfavby.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gnnzhgcto.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gdphmjbmp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gxfuefwkd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gpbszqank.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gfwywqekb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gsaqtbnww.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/goakxbzbu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gpwenmjfs.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gkixzlcbo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gxvlxroye.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gqcillzse.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gsmyaxnnp.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gqbyksiky.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gkzmzilrs.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gjlqumywc.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gqyppewmu.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvqlpzf.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gyvfvrief.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gainvuojt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gwimlttkb.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gzrwissup.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gpwfunecz.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gxssagjsw.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gereycdec.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gfwpfdifp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/ghxexwtjx.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gygeaewbu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gdpnwebwa.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gcwajibku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/grhhfilrc.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/grfowypvs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghjjgblti.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/grszfsudx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxefmqnpj.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gjamkwbqo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gzqkjfwhx.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gyitalvdy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gcmgrnowc.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gcnfbmmwt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gyeiuowlq.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/glrjgvhif.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gzewaaxcy.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/glbpshlqr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gntneipag.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gudrhtnqt.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqqblyiyj.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/grvrqxddf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ggpxlmwio.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gwdfkxulv.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/ggomavnjy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/glbvlshvc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gqcbvmsnv.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gzsijdpyq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gzdoknhwe.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gpallvwpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gnnkaslnz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwxhvogjm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gzgbaqnhg.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gcdmrpuzm.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/geyrpwwcm.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/geezxhekk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/grigrwuwe.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gsfohwdmy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/glolapidi.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gaonwzrwh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/ggutfgmui.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/godalqzlh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gersoiusv.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/ghoedlkol.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gtumaeeek.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gpkdgmlon.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gkjljmcfc.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gtsixwvvv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gvnuqnufa.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gesmhahds.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gabyngbho.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gyeivabne.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gmwrizymw.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gxcpsscea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gxxsrybzh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gxsjpghtu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gdfhfwtjx.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gdxhnwaat.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gjdzvmvdi.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/ggvoawvem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gscrhxgla.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gjqnxcrtg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/ggpsnsnyd.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gnuqcnugu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gcnuloypq.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gyljwjxfc.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/glnrbvdsi.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gwwhsengb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/grfbjanfy.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gmydaayij.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/giclvyyxt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gqqsogqml.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/glosevxli.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjvumovdx.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gpsdaeimz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzqfjdfso.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtablujpd.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gkhkradzx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gdrxkhuna.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/ginevjmjq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/glfswqiuz.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gqbuebrow.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gcqykxivo.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ggnrmtocw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gttfyfmox.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggzxeayzi.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gvnroqnfe.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gmfvxthpz.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gpgnbesfi.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/ghaevqsai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gkelquqfp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gvknvvaoe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gtiqryguq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/giwcuopjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gyjodlfki.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gvvolkvaa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gbprnhped.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvnwkmivq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gdgylsuue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gmvrfoacq.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gdqshpinh.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gjcvboixb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gxavtynaf.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gimhfxmsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gifcxhgxn.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gsglxutny.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gzrntmmpx.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gpvoxanre.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gefedlppz.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/ghrpoofpw.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gmbihjpnb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gpnwobiua.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gdxstfdiy.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gtxxdfhco.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gsdzjyirf.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gdqfhzoxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gblqpvusu.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/geiukkcgh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gkcxzgrkn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gsavigdpp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gjamwxrjb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gohqlluzv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gjmwevsiy.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/giqhfqjxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/ggxngerhh.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gdvlpkhtb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/giivfiyyi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gcdtevvgw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gijrfhifq.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/ggawzdwsb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gpvdrvmpi.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gaglanvte.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvqfptahg.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gzqhqoqmv.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gbmpcqzuo.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gvianhgkc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/grjtzguam.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gcwfadopw.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gkamrltbx.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gbncoyosv.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gtcubzqfo.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtvzpxuru.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gqdcqewvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gmofoczus.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gqaikdvhq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/glqainzid.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gyagugnhr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gkgbxumfy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gwjxxddve.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/girkyahai.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gbfvvflbd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqacnsbis.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gxqleryrz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghnzvzykm.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gyrssjhbz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/guwtolncv.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gbtrfchaf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gpzjtfvpk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gcyzbgrmc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gqfjfsbvi.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/glninivhn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gmbrvruig.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/glfvbupcz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gsrihkovx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gwsjckzqw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gprzbyzll.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gomwjmcmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gydybunjk.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gfclfuzrk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gtfsdwgnh.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/ghokieyhc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gvwlighht.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gfxmwezea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gagfcglcg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzghzfyod.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gzaqmwgpn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gajktpdya.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gvxanecta.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdowpqhgq.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/guhkndftf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ghjbxnzbe.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gdzjlhvoc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gllgmldbm.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/glzbzyrpa.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gbuigsmvc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gurqywdlm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gdsbjrsfh.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gyuudmbmi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gklknvvho.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gqxaovkch.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gxxstjlcd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gjnxvwnsr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gcnoyrgzt.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gicobmddp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gfjrupmko.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/grizytktx.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gghwhgiks.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gwgtrwahj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/glleiscvl.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gbbihgymh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gqxnjsniu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbqodrmgg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/grqkzpnmd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gidbrtvcf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/ggklropks.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glzhomwaf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwearkzpe.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gtsdyqbyy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gwxxpdype.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gwkkuxjmq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/giuqxcfcz.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gpcldpomu.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gvrjykelz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gfnarcyvs.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gbnyuhurn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gelnzdikr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxzwidojf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gxntbujdt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gwdkgccwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gsrnkenuh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gpknnyvix.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gzjvmzxuy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gkxhdhtwe.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gnlamovhk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gqdyfczil.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gsqzamnfh.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/guyudigpe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ggohesmxh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gonuebjyh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/geykyziwx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/grbvxvevr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gbwzeeipi.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gcmqlnjeu.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gdrhgobwg.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gpbfktwhr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gjfcmenbx.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gtcxhvqmb.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gocwbupwo.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gawbspxfq.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gjoauuqnu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/guobfebib.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gesnzcriv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gefydtbam.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gffllfuig.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gwohaycno.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gbdrnqgrf.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gagwelklw.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gnjpnakoi.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gyrnpocrh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gddwyspmk.sHtML


<!-- 参考信息 -->