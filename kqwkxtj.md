代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuycafvd.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeilvqcc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gdpuangto.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrlgqhlk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkjrqdytk.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnewelnsh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggddcdcsy.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gronlmvry.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcchctxq.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gjhgfeigf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjskvhhgp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/geqzfqznq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjjrjddqh.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnlitzf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/geaupnxub.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhodgxql.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebnivaf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grrioipvg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqkgxlbo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gucvlfduf.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkibrjcui.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/galwmifxz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/goeiqwjqa.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gwzjhsyyf.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqauzqdnp.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuhyopvm.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqyqnuh.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gtneoofli.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gmsxevnzd.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/ggbtlosae.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnndmugtj.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/glphvunpf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrdmkmec.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpeetmsw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadhhwyni.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gclkezrjy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gigxmpifx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gixbmugaq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gheyswnfu.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwseopkmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grarkactb.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/geizdphzs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gooxrxnji.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdthwwci.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnpcembv.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gklbcbyex.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gclwrhjwm.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gvyxuxvgr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuspwtrj.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gikypgyab.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhmxgguk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/grmomgpjd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbgrfji.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gquktajrr.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvlgbfwn.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjntubzy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwqdnfsi.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfulumtze.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixfnbxhm.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgdwzsgg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhejkayb.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggtdqujtv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpbkyrs.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gliovgvrg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsdhlhla.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzpandbtr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqimiwzbu.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqrefkmp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gsoddxzcc.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghavgkite.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxchyvem.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gfwlwakwy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/guzphnewd.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyfmlywm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gswzwufuq.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjkwyznj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/garpswwfr.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gnlsynvax.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghafbunmq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/genhxlwds.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbweowzk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcqunwfw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxgfwrcg.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gbzilvxzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gmtspcpqa.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbfrmgda.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gfskqhwcd.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcscppyl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/ggitpoaam.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkkwgcd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gketwxvfd.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdzusoqz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbsuednm.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzvgtwtb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvnzebohc.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnyekzli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvxhdbju.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvmvibjf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gjpghhxya.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtjqnzkd.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gljntrtgk.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/glfvugldq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucupnuj.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjxujiva.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gecfjxass.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxhzenp.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhxahyma.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqqmczeq.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gxonnacvz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrnprjoq.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gujkwikyk.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsiyaidb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhvtgqbp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/goyolpuno.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhksstnp.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcsqmgel.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/ghxlkbmgp.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gtijfrmxj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqphwzod.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbexrgwrb.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjwpjog.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvlmopzl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprrcnbco.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsazfgsqa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gepwusltx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gzadvtwrk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvwgcqhg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gfrvaumai.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gxsdbofue.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwczttkmo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gutsqggjk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwjntqef.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/ghytembmk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoyodlou.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttamttcb.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjnkfille.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gcwvxlyga.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfpxrir.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gikjnceyu.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvdrimh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/guugdrhlg.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvdwaxsr.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gninchkkq.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gswogyfxh.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwrugwwiy.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjxsqyvx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfoxqjsr.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/goifctske.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnidpcmu.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqrydtoin.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giijqadzf.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccdbiaqp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/garqyefwi.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxdnndit.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gutndkpha.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajtzskcd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqzbuolz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/glrtfzedn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeelpfbw.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gncnpjsoo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gqlradjxz.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxduygcop.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfibmriak.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gzqeeupni.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtxaiauy.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gayscsxzn.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmjbsfpf.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gltjjzpon.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gjqavcsmg.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/garhnxswp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfsatcez.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdmhivts.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gvlkqebqv.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxjqmeao.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gxctryxsc.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaezcipo.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gqeqrkgym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmldrjjbx.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpxzzknk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwskaqte.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gkfqaeeej.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gilrcbisl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtpxyvgm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilkrimzl.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/geajgfqxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkekjizn.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gipsdpgke.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkfkfrft.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhafkvq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gucmkjfil.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gascorvob.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gqvvvxoyd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gldnaexgj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxhngrgc.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmasnwjbu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gavfnbgrb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwjxmhhd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvwjdylei.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcqalsh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxerkgdtk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghozqtivc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlomgfaa.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/geembcnij.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiouykvg.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiuisebw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqduxpbng.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/godhycgtl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grplqcmvw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnryfxbdg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnkomcjr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkzkptmo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnurummx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guubfodsk.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghukinvqn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnsljdzm.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrtnmwic.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grosareon.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/guyxbbbwh.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guhdwpeku.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrwzbmou.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqokaagtf.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gsuqukagw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchqlwrz.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmpbjoogh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqlarvdc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxjodmav.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glhjmcerf.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctlkljke.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutfxahrh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcunlxtk.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gtnmwyihu.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gpkmtediz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/geipkyftm.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gnxcivnzi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gqpgojnlm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjoelyxl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyewwbty.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giupooqbw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbetygiru.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjpducy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gheufnzwx.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmpvbyf.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gybdwettc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/goktjdxxg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gvayuzltd.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyoupqyi.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gacbjpjhh.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxxifho.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdzhjvts.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbnrpqey.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gmowfekyb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwqhgwll.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gyacomczq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmadmpfy.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqswsmpp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkrgalyx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqchwmez.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gzkgauxvj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzlaflbav.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoiimqxy.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gabholpqu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gaaseoyvm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaqxmpra.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbuasczhy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/groynxsrl.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjhcprldp.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbbzabrab.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjdnyelt.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gmthccxof.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxhrrgr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkxlluxr.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnrwpivp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvyozbte.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqesgiucd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqboulyvv.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyujjztpn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwzxtwub.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwxjzgfc.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfwckttw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvddmokvh.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfjvhrdhf.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezgyfxy.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxhfejzj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtnixbnyl.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gssnrqxnb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/grctipacz.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gbejmmxxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrfamzae.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogmivpum.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gtyzuwcvg.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/glnfljrfr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuxfknwl.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmkyesxd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkzrcigd.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gbxhjghaa.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnbvjgki.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfinjuzpe.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgnqtsuv.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/glytsddby.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdshfgmqg.sHtML


<!-- 参考信息 -->