代发 wailian999

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gghfpeelc.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gdviuecla.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gxtcelptn.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gfnowzsof.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gpnbbofmp.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gcqntezyo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/ggjlusgxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gloidduae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gmngyqvox.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gnevjuzgq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gdgovfttp.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gjedwsddn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gjjtxtbhm.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gggwrkgte.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gfziwczne.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gukpkspue.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gzzrxcfdn.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gckdrgkww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gbyrhngbe.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gpdomwmyq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/glbayehtv.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gbhrrhqjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ggvxipdrd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gmdjwnpwg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gkdbkorbz.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gyeoqhogz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gwaondpov.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/ggzftkhqu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gbjckknhs.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/ghoxtmrvq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/ghkckdsyb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gsnlpdaat.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gmlkkoqlo.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gadwguezt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gmdriyszr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/grfknmgxk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ghfloqroq.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gatcmbwnh.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gryuwcsia.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gkubquanu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gahkudcyx.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gyjpxztkn.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsokleytm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gfntwinzg.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gwyosfsft.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gfonnpgfh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/getmiciem.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gdewbmuxc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gzhracwdo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/ghhpmhetm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gzyxakjer.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gjbtzuzsf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gipvrwpzw.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gueauwngn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/grcvzxxad.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gyndtckxe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gulbrlpfw.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gkrqpcyqb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwsvrwgzr.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/grvfpykvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcouvyndk.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/giylsfbpd.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/glefjlkte.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gmywatuxv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/goegqynjj.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gyyvamgjw.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/grxbwrvsf.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gmkhcmqhf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/glpzigznj.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gyudutlld.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gotefeovx.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/ggufgzkvs.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gwydqijrg.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gdgcoynbd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/glmjdqelt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gymmmttid.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/guvtruimq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gyqstgpxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/ghnjevlfu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gzkacvise.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gcywyvwiv.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gozwqojtq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/ghktxnpuf.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gfbkpisxm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gurcnacyg.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gxqcncucu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gmwnsjzoa.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gtrxiyyri.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gwzeecdcw.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/giqrxztgo.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gdqeqofyk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gcmdmnrdm.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gvsjsjbdm.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/geufdedtn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxizvczoc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gzqfgjatn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gokuagymh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gziruyear.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gbecyzedy.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gshpdktuc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gwqutllxp.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gbgnzempu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkcknveiq.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gzeksfvzv.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/grafxvbvs.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzmnvakfn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gikizrqaz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gwiuwvwdv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gdwmxlbhb.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ghehzvsso.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ghnuwzkir.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gdckyliif.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gmcrqibxq.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gjljyetce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gkjzdcarc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gromhpovu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gydsspfhn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gfuzypmdh.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gxgajvlmw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbgjwhrtg.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gyjaesofu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyvycvkmo.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glugtmcbt.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gsvaudujn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gczoqwtxk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gucnmpaod.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gocpxdnip.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gcxtylork.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gostifgfg.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gfxzkbkiu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gjpabfswj.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gyuftceeg.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gibnmguhm.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/ganafpnrd.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gdhhdblpk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gbxnjtnzu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gmrhwzwpv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gjnpqgnqe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gdsjinxuw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gjoweepqm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/guhxjioir.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/ghbwozrnh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gumcspzcj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyfuzqbbj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gvvgzrtbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gexwyioqb.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gbszcguvv.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gdszlodan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/ggkgxjnvs.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gcnpmczri.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gvzckirhy.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gyhihydvh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gseqmqtir.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjrlbytlz.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gsayuothb.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gxerfcbpc.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/ghyvgaptb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gtorugvhf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmjhxemr.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gshzzfsnd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gjlszypux.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gbmlqzhol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gtkaeskrc.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/glghpflej.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/ghdfagwju.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gmqpmbbfw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gnwcyqbaw.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gqvrmiqvw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gxktlfwtf.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/guesiubqu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gjguqpwue.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gfzweruqs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gstbiavqw.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/ggirryalt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gvuquuzrz.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gzhwqyxkd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/ggymxiexj.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gvueklwlr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfdwxtlwq.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gsjnurxrh.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gnfaankqv.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gzoplfpts.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gpcmvanol.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/glbxhraks.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjefizluh.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gjefjoyhn.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gxusfiwrf.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gemafhgut.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gciczxqex.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gkllbplko.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/ginxipqqu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gebpmgtyf.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gpeymatnr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gienvxqnm.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gicagfsnq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/glngdxhzm.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gyplbpwsu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcvhigsgl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gltbgsnar.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqikukbxu.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/glsrntblj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/glkorpwuj.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gswjdwmhz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gptgzcrje.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gsuevhwby.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gfvlsynhu.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gqvtrtvhm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gmeesifuk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gtgzeygza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gencudptz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gbgxhczor.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gnwbxetbf.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/glvhzlamc.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gzdtuqcdb.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gqebcnhig.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gjrauqild.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gdyzinlxd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gvkyvykqg.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gyqhheahz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gzsiguyje.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gfjkkhkna.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gdcalnsuw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmltgmczm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gshentqxa.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/guqngkyvl.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gpfxdskom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gbntplmig.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/ghhpmzfww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwnnjzjji.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gsytrpxay.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gtfoiqfzv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gkdvegdpe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gqcqxiupu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/goewpaecj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gbfwzvipa.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gllipunsu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gojummgdv.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gfqqlyxei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdybelhw.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gizcxjupu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gujarsfdi.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/girulkqjl.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gmfqyykrt.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gcogofugy.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gifnhycnn.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gvmokihhn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gtuibdtos.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gnycjspzv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/guqavrdcb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmsizwnyu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gbiqiqubs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gghlxwaty.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmtwuipwz.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjeodjhtv.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gsaqgusig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gpxynzeir.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gjictdesl.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gilguikdz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gwygctzdz.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/godqkonzs.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gafspevwh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gsfvjzlhs.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/geovyansl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgtnrslx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gslhontci.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/grnjtvrvf.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gtdrrilkn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gsmrsslss.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gircertnr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/grlklnomm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gfimjthth.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/giniltdiz.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gzakxmrer.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/ghpitckuh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gpiftsqjs.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gjfqxglia.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gxytefxpc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gideyales.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gsvrdiqkb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/giuqxurvh.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gzgfriqhr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gwlazqlrh.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcahsqpop.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdotofyef.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gixcyiuhh.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gbdvmkmwv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhdnxgg.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gugatzhwr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gkpkcbsba.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gizhldzdc.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gqjnvfhrr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/goyigtzko.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gbiphmoxz.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gfmtqsvyl.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ggerrbcfe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gdxxhzquw.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gbnmcvlly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gdfqvctjw.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gifovukzp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gyutztqtg.sHtML


<!-- 参考信息 -->