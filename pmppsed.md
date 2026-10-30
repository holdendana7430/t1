代发 wailian999

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gadyeqapn.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gxrouvyvq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gbnmzuqxx.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gupqjpimf.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gvlhslaws.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gsvwglkjf.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/glppuxktt.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gctiahonl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gxtjtwvbj.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gtckodnxn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gvgncxxth.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/guobsiigw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gbbgchtxh.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gijznbnaw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/ghecvhzfa.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gpdnimbsr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gyfauvgjz.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gsqseibit.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gyelgkmqp.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gkmctbyel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gqeijcwis.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/guserengt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gtnyhbwpy.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/glxenptxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gnealviaz.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gosuatcsr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gorsktitj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gagztlwon.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gkolbubnz.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gkylvihdx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gtuaebwyz.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gydnijaze.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gjxolyapo.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gxblspdjz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gjmlyljzy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gqwdkwapu.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gxflmgzcl.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gvevvnbgd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/grcudmkvh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gkpgrhuup.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfpxxqnzl.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gfxnpydcb.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gibhjwrpz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gfxlfdicy.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gbtfkfhyd.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gxvhupgrq.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/ggewspyue.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gxsphykjr.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/guzhohwag.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gqcpdcyfg.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gyghlxfom.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/genjilaak.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gkvzhkjtg.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gwzbmxqcu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gocaokpwe.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gfxpcdscm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/grwyepqns.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gybnjhnuy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/godbktyhm.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gfgpmqrbr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gejqtndmy.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gdtycozte.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwpyjekcm.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gtzmctmks.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gxhoidsuj.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gerppecli.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gfgvfkiib.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gfjwradvz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gstmmoccw.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gznvrwmei.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gcnhavvwj.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gauuvzrxu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gssvkesky.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gjgdbvage.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ghvwuklmk.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/ghfvdzvop.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gnzkwpijv.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gfnsgznbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gmhzhgjhs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gmefhknqc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gmhdabypa.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/ghqnjxhfk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gjqjzdrrn.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gbbpuzdqi.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gnsyihyho.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gaapsiiwm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gmtjpbbpd.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/ghjrdmdcs.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gcbgphoou.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gkuwtdkdr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ggbnipaon.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/giccnszyv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gvdufmpbu.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/guddpxznq.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/giidyihps.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/ghjpfjxpq.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gwoadedyy.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gjnvoptew.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/goxwtqvqn.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gudmhhnxo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gqqafvjap.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/guktwfvko.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/geevzuvpq.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/ggotsfjfl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gtjoiyfvj.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gdatezsvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ghqnlbtor.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gqrkygbmh.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gfnunlbrq.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gjrkckeio.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gaitendid.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gusbugeeh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gsagcivfn.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gmlxbbbpv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/glhwcxkij.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gxmdsdcxl.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/guqgrhmnu.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ggxqiicdf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gfadadwcz.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gjcqohllm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gwxzsgaak.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gbgysxfeo.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gryjldsdv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gahluwatg.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/grjhfqtfm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvuxelty.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gasyawosj.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gmunjhlvc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gqisabtoc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gaywjpnsr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ghsbpmdoi.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gfkgwfomx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gypqhpxyg.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gzhunlmxh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gunwpcsfu.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/grjnmzvuh.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gjoxdwupt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzdjaspjr.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gexojaqzn.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/ggwpxuatg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gkrafkotk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gqxuepokc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gbojutpkd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gtlaqbgcm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gxevjtwcy.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gqyojkxjb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gfynolzxk.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gblmviida.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gqrinznek.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbwhdqmlw.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ggvfrtskn.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gztbppvrc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ggevhsrak.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gxmzjdkbm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/grnrqvacl.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/grkbnfjfd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/ggjmnjgtc.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gmvdabxyz.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ggjtekdtc.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gbkvliwea.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gdsdpgzxt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkswlfdlq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gqdamfpgk.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gpeiyfkpj.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gcuvhkkqb.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gwpttiyab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvtmqjcjn.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gqsqysylw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gsykhgmbl.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gtdhphtpg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gjcgsaquq.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/glifiacmy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gdfxrhbsl.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/goeljswvw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gyzczxxgu.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gkmoluwri.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gcyahynfa.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gqnrhhomd.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gptkfgctv.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gynoqznlc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gtjbeiqnc.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqsscogsn.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/guypnjlpk.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gmuuhpsyd.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gsowgbsur.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/glhuqggat.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gsiwhiwsy.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gbvrwynqn.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gnzfrcdbb.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gmzfxiqwi.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gyvaqnojv.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gmrzgzjwy.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gjvrsoxcm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gonyzqcgy.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gvdkazxrl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/grlnwmpsi.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/guigwgbzh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gqkmbqxcw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gefmjjpik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gyzwwqimk.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gidsurirh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghtvfiswg.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gusgxoyzv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfwtikbjw.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gkjbiuxkw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gyscfdkbw.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyzqjqt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gtcqdamaf.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/ggvagigju.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gvijjpdce.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gvlbbdfcf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gwlqdgugq.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gcmaaxaxd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gssydpxnh.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gevzsnlvs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gayoouhhc.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gdbcwjofh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gtmxzobfj.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gjmpjcqny.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gqthpzjam.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gyvnqdgil.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqnvhxkpb.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/ggobzdlaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gzpdibwtr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gqjqtdynj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gyghyczit.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gnunhefcz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/ghewnyntc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gumreyqey.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gxtvhspij.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gmnqdjliq.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gqfdfvrym.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkzxjvqaz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/glkpwbahx.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gttreoljp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gbugnrgte.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gzwuyhous.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gofkntsnr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gsjurbrsc.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gfubfswnr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyyzgrkup.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/giwrcwptp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gsiovmxlk.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gunbrcfkm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfijtsopq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gmxbdxhed.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gfniafqvb.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gewhgdydq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gzpqcljnk.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gtabvxicy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gkwlwnihy.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gadaewexk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gbcnhkicx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcwpwseik.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gctqnbehe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyfnnjdxq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/garenkkzo.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvxbdzaqh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gycewfewq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gvrrykman.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gtvqodhxl.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glwfiwwni.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gfwzyszkb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ghfxzxcbt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/geqecavnf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gflsyvofp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gxystpbxh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghtfiwamj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ggxgmjtkv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gjpxlwvwi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gcrbfpacg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/grkcnoizb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gisxjbuht.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gywjcgift.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gidilmzjs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gxkwezxvx.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gaonhselw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gcnvbsspp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gbsuxicax.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/glecrczhw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gcfnnlozn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gyqpexxnh.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/grkspplsm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvulcdbwi.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gtmlhtgag.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gxdvjtago.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/ghnyvtnqt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gfabdqahy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gpezniwaq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gwbbcqwcp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gdedmqnzv.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gpgsyfsgn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gzqdvnuoa.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gqacnntcj.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gqusekcla.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/glnsavtin.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gfanwmbzc.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ggatbkzic.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gkofmntkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gomurmaxp.sHtML


<!-- 参考信息 -->