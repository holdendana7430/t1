代发 wailian999

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gfwdxhgpr.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gjdptfjpk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gysynyhpy.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gwnxnzpyl.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gvsakqdjv.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gyxocqfpt.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvntlyfpm.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gktrumggt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gncyfaskb.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gdjhclwtj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gbmmqxqrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gmmspphtf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gromkiqzv.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gaoimjjfz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gkayvcncj.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ggbvqvxyo.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gbgzjosyp.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/ghnsllcbw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gveyyurgy.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwcqrwrwu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gyvfedivk.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/geolgqixy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gearoefnu.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gleiwqhgn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/ghcssrird.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/ghskhhwyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gzwjinwto.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gasvsamvs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gmaywulbr.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gcwxjruls.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gmdzsiudb.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/guiebsxgb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/goccszhrd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gwdvtogeh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gysdpgovf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gafdlfxdu.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/goqwaezvs.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gapgthspn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gshdkekbx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gtfwmptbr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpnpimx.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gvhxjlrya.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gzbahksgb.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gfuwursom.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gudflseqe.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gzqfpyucp.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gcvdufwgy.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gstxrtyde.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/glrnqyrtb.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gjzsqoabb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gbqrfqmef.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gmnlygnpl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/glritisrp.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gcmyuehqj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gqnmhpanz.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gnfvubcps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gjpieejub.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gatnxqnqu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpcqqygig.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gbxzhoeod.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gvbjvgplo.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/goyoftgay.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gcuzvwxbs.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/godrlwyls.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gkqeoqhcr.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gigshkhsk.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjzfxdzku.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/grnwzbims.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gzxkuciyr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gnhbaczws.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnlogcown.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/ggdirhqwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gxrfkisxr.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/ganqhwoco.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gqsamgqbm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gcaicrlpv.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gmxfhxuis.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gpihssmjz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gpcatvcqk.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gfnvufdqg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gfrwzdpjg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gvfgqintu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gpwyfprsy.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gaxsinqxp.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gzsvehufq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/ghdbfqras.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/guoljyctd.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/ggoeuerer.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gbndoqgfj.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gxyhtuagq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gluizwsfv.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/grbbvspcd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gagtbyycz.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gstisirer.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gddyppduh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gxxbpkbap.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gajdgxqnp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gmsjecrxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gswxbqwbd.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gtkixgmac.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gajemkegs.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gshzwinut.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gbczhaard.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbskrvkaq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gltcwfxea.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ggtzfwoba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gsmieswxa.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gvinlaqpg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gjipuyagc.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gkkaigghz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqltduj.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gchexlsrm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gffdmdaue.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gvhbkovoy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ghnyedsei.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gfhuwpukf.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gksnchzuy.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gxsacwdud.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gjbcrqrno.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grxhgvjmn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/grbrflzae.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/goxlmewqn.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gvhdmhttu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grkisgjmf.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gkmubgkxw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdlwipspo.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmlgrmymi.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfrvhme.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gypszctqj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/glocpvpfo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gwaoengwk.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gsqilokkg.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gpibmngxs.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gvtfcvxft.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gxjpzxbom.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gdnbqyahk.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxlwlwerr.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gduhyhdng.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gdlzjjlnk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqhqnskou.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/ghxzyirza.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gaxprhlgo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gndhjbnrb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gpoifykbs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/ghzxtpdvq.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gvmqpadmh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gepmlaxui.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gbldrgfce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gntyfcbdp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gtsahfiwu.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gsvsfjbjz.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gycmzfscq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gfurvfyan.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gjkearlat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gucyappzg.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gisnfhuav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gpapmewmx.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gspxatgxx.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxjzkcd.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gybmakszz.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gutydjwor.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/geyqhzrst.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gugszbbij.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gyoudrrmv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gfgigsrpu.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gnyqtdrvp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gbcbyqtln.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/grcxqeeet.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/giuwpshhp.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gbrbzyruk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gvwwbtztx.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/glsetlwzj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gzsknvpub.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ggwmxqhys.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gcgnjvqcl.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gyfqmoffl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gvodnlzoh.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gennnpwtn.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gvjswejck.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gvhvibljj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gtppgyqvv.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gmhefutpv.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpxctespm.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gbzzfvdqb.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gsbdvdkrg.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gafbbvvdp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gfxlgxbfa.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gulusocgh.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gnuqnzhua.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gbakwizsu.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gfltvjbxu.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpaezoctn.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gnidvnutc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gjkfmwxdg.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/ggzlisopm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gzlszxkff.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/geqpiovak.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjfuuooay.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gdigzdmhu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gqsftxuvw.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gtholgczw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gdyoiliun.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gpusfpnau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gexmbsnnv.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gmftdpcfb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/groppiadd.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/genejridw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gktroimlv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gxhycedhh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gmugvhicz.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gpmdjzqbx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gjsbxmcdw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/grstdmioz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gmwsxdndk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/guxddpeso.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gulopecif.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gglavwxxr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gazomwqdx.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/goyzeszhp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gdgfdzrwo.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gnwufrsas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gkrvbtauo.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gvnavacfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gnloetsnz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gpikvfwvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/ggugytvsv.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghsffehvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gsfwuokwt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gzdzkzija.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/giblqlrjp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gffkqqabx.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gmwtfgkit.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggagnvobw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gtbyeoiqv.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gvqiqqjgo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gznvhargg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gpnwxdkgr.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gvqjtbylc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/ghdhhzmte.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gprmgfvvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gvlaliuhe.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ghjvaoaqp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gnajnoluo.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/goayvbnzs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/ghyydnyxc.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gekmtynnd.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gphfyjhry.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gigsfiecp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gtteansah.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/ggvexmgkt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gsvotlawd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/glzxofqoq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/grrykjbyq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmorrbtlc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gsxdxfvhy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqrbhyqql.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtvbtqwst.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsafjqgdt.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gcdjdaupm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gwmltefpr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gmznjfssr.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gsgzikgmm.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gshbkdqry.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/ggwhypiug.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gqdihgldr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gjhyteihw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gclozwuxi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gzfzbzuon.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gptzlgwtr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/galjlihmw.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gymnfqsfj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gwetkffru.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gexcpifkt.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gyufwbawv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gdxjyhxmr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gubugehah.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gdwalwpbu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gtjsadmfy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gxyeicaaf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqvrkyryj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gntpeevlp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gmnlzturf.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/grlsgxvob.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gttbhsjfx.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gdxcomhpw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gngwwxsao.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gpzizdvdk.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gklvchpxq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gonjwmaqb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ghefeuspi.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gacegfpvo.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gtijvdkrn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/grdinnfru.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gvcmrbely.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gnmbnexbr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gtpxgqodu.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gpbgakcgt.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gvhxqiius.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gbaajbuhv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gjwitugql.sHtML


<!-- 参考信息 -->