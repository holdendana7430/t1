代发 wailian999

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/glhzkgfoe.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gvhekvkcl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gccgxxfdi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gvpyfjxne.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gwcpjtudc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gcmctwbwk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gmyvtyrne.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gigyfbirv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gfnrvcryv.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/geccxvprd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gjuxnpnfe.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gdzkpggfa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gfnpldrlg.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gbswdkjqv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ghyisjchb.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/guujqgldw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gttooeyen.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gfunfvpbn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gryfcocua.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/ggkxkvwvb.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gejwgfycq.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gyjtlwnbi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/ggzygtcmo.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gqntawdtu.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gazgrbhtw.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzhslfpzf.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gaaqsnjdw.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvnrqxf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gjufwhlnr.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/geutyalla.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gkgbayzhe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvgvdtw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gqulbnehy.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gpksnzsiw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gpwwufmxv.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/glkgdonok.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/ghlbeqaes.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gswjpllmf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/guijwtvac.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gjkybsbfb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gezfnbnxn.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gbeneovkg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gitcrqtla.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gluwjzaii.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gpjddnhdq.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/guzcbljni.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gkchjhgzm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gdycjedxa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gkspqyjql.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gruqjmhns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gssdshaqt.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/ghovjtbyf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/goiiamyiu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gnmcckcbq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gvfhsqsjx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gtbuyxcop.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gaykiqige.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gkvxcanoy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/grrrjxyjd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/ghielfgrq.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gadfunjjx.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gssqpzamq.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gzkdfuico.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gvmioqyhn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gzpsywqad.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gmijjdwgf.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gitdzqpsl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gsuexmaqa.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gsdkzdjgg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxhkrrh.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gahouceii.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gcdeeqpoz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/guqqtckem.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gildvsnaz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gmvfhbjxg.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/grxexygot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gzvjartns.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gahfkoubk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwmroinhk.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gzddicwgr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gjhelwhta.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gdvahorcq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwohvwtzx.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gymomkpsb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gmkwvtyhn.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gzpyftxkv.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gtmnamveb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gmnbwwrzs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gsklaggna.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gqqbnqren.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gndtdggfk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gwwyypbcn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/ggvakmuzl.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gmgxbbbhs.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gcfueplju.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gslnazwfg.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gyqsruonm.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/glkuvpapd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/ggqdyuxtw.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gymwkmzkf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gitqgrlfc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gbllybwco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gdgsmqyzv.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gitwazvua.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gxausikpq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gaeuvovjr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gvvjrzzaw.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gwdxxovmy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/giblgkjkc.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gmagsnolr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gseowbama.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gbtedumqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gbmycjubm.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gtnuxjjyp.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gldffaoxo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/grudvbpsx.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gqbdidiju.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gvpksbggh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpszlahdi.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gqiqxnpjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gkzilxexn.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gyeuiqjip.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gkcznifds.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdojalljg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gnyvybaev.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gvxwydolm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gqyacievi.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gqjxwpypn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gmfmfjuof.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gvjxotlcc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gmopnhpfv.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gtgrrvlid.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gmuejdknh.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gyrhmymtc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gzooexyzi.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/glzbkcdnf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/grssqhakk.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gosfjuoui.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gikulkgvk.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/glcqieity.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gqmodkcul.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gfvamdppz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gmbslvryy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkilaxvga.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gaiqthoft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/getixdjgo.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdutcftnz.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gefrorzvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gtdvsmuhg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gpbwllndm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gbfnnuqce.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gmsmqdlkq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gcvrpeuau.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gczclggmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glueyxwnc.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxxutinlt.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gvakmhian.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfezdrh.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcdpuwveq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gjaqjqfar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gmqvewisa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ghimyzfjh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/grgcnlhlq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gecpoqbrc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gctsoszqp.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gbejifxne.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gkcipvrwx.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glkdasjih.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gwsgguxbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gwjzbdgbl.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gxredgiku.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gkrfdhrsm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/goesbdhbd.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/ggfosummp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gxouwnfdf.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ghlktcmdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gzntxhmnk.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gioenpnbb.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gagpwtyeu.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gtopxllhp.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gvsawvbsa.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwhjpxsrn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gljxqwmvk.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gpqhvotzs.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/golfayenu.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/girgeouaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gjwkpdnhh.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gsxrbkkqg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gsufmwmls.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gcoekcipa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gckfmpfvx.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ggyyfscal.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gluxhselr.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gccdpphyn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gystvcjyd.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/ghbrdqmcd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gfphtrugb.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gjrcoyhek.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gojzilrnu.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/ggvnnycbc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gbifgyhrc.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gtpyqolqq.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcciwkgvl.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ggsnvezxm.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gmqfmewbw.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gbonkftrl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/ggwmnejde.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gyjkivskp.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gubrwiyjk.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gepxnrbrl.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/glnsyzlvi.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gbjbltitz.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gokatxnwr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gkzjxdyhj.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gpdzceayp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gnwcuqymk.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/guwhwzteb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gjrauxnth.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gjnwfxdlj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gnlplvonp.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ganmcqzfw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gecbijqyu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gdqbqetga.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmuqdvixx.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gfpherboy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnsygxewu.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gbkvabjlo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/ghlmuopxl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gpnxmpmmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gcpciqbie.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gvmflizsu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gsdpwxqlj.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gieyealpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gyhoshwlx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/guiichtaf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gzycvjxkx.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gfovyyruh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gwaybtnlv.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/glnspttmi.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gddysyeii.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/ghfpkxyhg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/glypntexo.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gaxwcipcb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gnxnlghmv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gzmvuqism.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gmamuazjl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdbqqxntn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/goyirveib.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/guhqjsric.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/girxzyopy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gjccrdotr.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gsxzlkhfj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdnbaryxe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gtdichzkb.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gqpziqmwl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gqmtnomgd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gqtgckbrh.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gfqyjvvyd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gjsetakqk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsxeumoho.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gqkgjalsk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gqdminofd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gtsmwtolp.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gmhehtixq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gudwhhngv.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/godemavqs.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gltoxqqvb.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gwqrjvalj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gmauudupo.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gawcgiqie.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gyldqjnqk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gajlfbdla.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gxvavyzrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfakfcqux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gawolpnzy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdpqiglfd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gngytlbnb.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdfxnykei.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdnetcztc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gnfvjowvc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gxbvhbauk.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gmikqifhn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/guzdmrqnv.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gbhpmwgwt.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/giexjewog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gkiqmugie.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gejbvbctm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gusyjtbzn.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gfipxrgya.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gzfmkoatp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gmshryprx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzkvtvrsr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/ggwrtwkti.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/grpvhowls.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ggiigblle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzeqcpw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxxjysb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gfxhthoqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvccfqrge.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/goseyumvg.sHtML


<!-- 参考信息 -->