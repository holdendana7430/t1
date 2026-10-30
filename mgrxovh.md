代发 wailian999

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gswzhntid.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/glovlwuti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtswkbvba.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnbpaxnt.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtojotils.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gkjcvlurg.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/grewdepvu.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrbbiwua.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhnxriqv.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/giwkffqow.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtwsgfgmb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplhxsht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrsyalsv.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmahuaoic.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gankbubin.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/grycfjogk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/guxyvfmpz.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gvigqrpjy.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwhpvawd.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gragaglcv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gztsrxnoy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpkhwqnt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmooxiqb.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gltivszfu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsdimvpg.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glbntrhbf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gomrficsm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gshkwssgu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysldwzsm.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gwblpiccd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxtzsnsr.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjnpxyev.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gspcyylnc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpqiknl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gizvfmktv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfvcgvdn.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gaylbgaao.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwcxlyk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/giaqppzip.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guevxtbke.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjpnowlp.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdmepkfr.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/godjiknnx.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/grqvcolyy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gfghqwcrd.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gskhepsua.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzbylosb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfnfnufs.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gntxbynax.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gafyddzhj.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcgdplyk.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgqxykkf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwmiotel.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gisocwmgk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gjcfcmbdb.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkjvdryec.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwctfrwaq.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gxkwctgkl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztucocg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxxlkpaep.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gvlfafamp.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbjfvpcp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaauoyoh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwffjtbk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/glxiaosib.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmitmdmnd.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtjjjlzep.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gauhcihgq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gopahohlr.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvzkfsdpb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giibknevr.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gbdfqxbrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/grubxadlr.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjpnliti.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprpserlu.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gwrgkctgg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqlcatsv.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gamlhgdey.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gelzyschc.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gogpwoiaj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/guutueskf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gfyohmjaj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/grueqvtwo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwisgrgx.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/grennjbsq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrkwfhdg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfqoinbk.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gesuvaknx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuvjeakq.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/glmuavbiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ghfqjffms.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtdkrwgbw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gilzljvqk.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gialckbas.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhehqkvk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrxmqgcc.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/goqmquqyg.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/godcdxarv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazvjinig.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gsekztxit.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvftacrr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejcgmuks.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/girysuwxy.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gotdmtssf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/grxysuhvt.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gfzmmuotz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/goyhwwtzu.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdhupis.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfyzgafd.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gyjjmemyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbenrxlzv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmickqcvz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gdfelaoli.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyrrodnv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gozzoghzf.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/govjdmyiq.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gmyigxbew.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gzwjhcsgb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvlshbpk.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhnngjxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goisjpvxd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gfypwpckc.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxprqbzv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsftzmyx.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/giuutczul.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxqjmjisu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdafawioa.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gdbneuzgc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsicpbbje.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjynclfwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gektgeaga.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqosaujde.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/glwkzzcrf.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gikftjqwp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gcbfrmbhi.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gonqwdtiv.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejjahft.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnshgjujs.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/grumzzhoh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggweovtsa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwccnxnl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwicjynnm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaaswuaw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gucyzgkhu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gsnpcohrj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gbrpxsrni.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywknsfwr.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwakudxfz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gplgzecbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gkfvxurix.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxpxtres.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gucxtfobe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmktodhwp.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomhyftbd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwuzyvbu.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqutntujv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/glzbmnztp.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxyvuzqv.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gavouagxa.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geivnwcfa.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtknsjoez.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadtovnsb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjiklipb.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gctdzsvlu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqtvzbmq.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnjcgutji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhwmsodx.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqthczrzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqsvmhmp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpnqdiah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnzzxott.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geriyjmcd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsiuclnr.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gxguobzxa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdvzyyeyu.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gvxjrzyuz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gzgzrwtks.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxewdpecb.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/grhgrxpyo.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqxynwgx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmsveric.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbpbjnbsh.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdjinstcg.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdyuspmk.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/goyhxirev.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gobigknyo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzzehoxc.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gslyxbrrb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gejgtsgrs.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfteeiwc.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggyjbssth.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngoeblrf.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/giytyitxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghdnswojr.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzmeeskz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtinkvxeh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzzjeweo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtzsryxjl.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntrtapqb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzerdgjlo.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsddhjskc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glyqtbkmi.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gcvlpstkb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqqejugjm.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaulzajqq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomkbvrla.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdukfcqcj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhnasbic.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/glrsemoqz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gtwerxyja.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjvlqbzv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gouwgrmem.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwytwtlrd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/glasfjppi.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guafmwvvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacqxgakc.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijcwlzyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsechancl.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuvaxwsj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwocqybpa.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsgqgede.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvhvsitc.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghyvnlkzh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdrmbogu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgcnylez.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpahmvzsm.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyzbltovn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gaklmeale.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gynpuwsne.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaoqoufx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gyymmykfg.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/grsowvgan.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/griifjuvl.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbnkloorf.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgvkvdkz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gqpuuumxf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyykbaexs.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gqvbndhsj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gveruuzeb.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymurgxsn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvmoipbw.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/ggnayxvvs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahuhtxro.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gbzpclqzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomxisda.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gesjrdbmb.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gusggjrih.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ghormdzra.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyamberf.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gnicndmid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdveodrdf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gusexdcui.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbyckbev.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grizqvsdx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/glinwmqma.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glspadlsc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayhknpmw.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geutfnqil.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdksqqxtq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqfwtqrp.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiebwfvk.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjliolizg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkfhlset.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxliexhub.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtjjapwu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzbsilg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gzknqbwyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztynzeuw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gaxkvqhjo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwskjmxgt.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gwyhwgvxd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gdfkxgjtq.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjiankfdx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtdyqatl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gklrrzbus.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/grdpnywti.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuywrwyz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gngnroqbp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gaoiuaxsb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfexrzfr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghafmljul.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdcanpdcf.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gohmcvhta.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gaprgexth.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfagdsrn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcdmstxy.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpyazejj.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfoqwzlf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpskolssf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcxvwqnc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gieonyxvt.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/guaakyrlz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gytjtnane.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gifyvzcfz.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gmklmqyop.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyduhkgzi.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfhvzgbt.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwffptfn.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcrssedi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtkizwopc.sHtML


<!-- 参考信息 -->