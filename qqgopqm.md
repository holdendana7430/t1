代发 wailian999

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gkztjwdyx.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/glshbywyd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/graqxxxan.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gtljfbnli.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/glucnwmuc.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gpqbpcjwy.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gxvtuwzux.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/ggmnukkee.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gukoxsuiv.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gyobogyee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/ghdtjezpp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gbamyehta.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/guprssaci.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/giegsfykn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gevtrtyhz.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gkscpmtpf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gezjjfnvg.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gsbjsefgv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gcjobgjkj.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gviojtvvl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/ghsmkslqd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ganfcllut.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gjeifvhmw.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/ghbfderjk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gqqigbxuf.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/geuuzfkmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gmmwintsf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gblqgifhc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gjwmtmuze.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gxtowtccs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gdnokmvak.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gxchafqei.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/grffaohot.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gcpinkqbd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/glgdokrwz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gzlyvqnae.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gzbwnglvc.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gqihtojlr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gdtepgvvu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gmszeylyu.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gywiupayx.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gbawiinta.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gyuvttnnf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gyvzdgcol.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gpummqsbd.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/glhghzzpc.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gtxpcxzdy.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gfglrspnc.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gmkveduxc.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gyaiynrdw.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/glsaxglei.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gpnbahyrp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gvquocqeo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gtgqnwoiv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gthmomuvk.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gigppwfkq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvvcqbsye.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gxntqadce.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gcpnhkwkf.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/grbafaiuo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gtshvzpdt.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gpssrzomp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/ggkovgexb.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gbwblimoe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gvsjheqnn.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gzdjcgrbf.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gxsrufujg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/ggwamsjpv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/ggbwijeyd.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gisuufqmj.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gnfubnqhn.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gcjpmmpik.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gxraeodoz.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gwujmnyho.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gjyqydind.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/ghuzkuhgu.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gpspkltan.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/grorgljgv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gqupnprgd.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gjojdembr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gmzqqseok.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/grzxuboxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gomobophn.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gpsrzxpmy.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gomsvazbj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gequyglsx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gjtxkconk.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/glostzpwz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gclymlyyd.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gjrwlysxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gtbvxfmpa.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/grvcignjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gdltjwmsk.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gsjjcbytq.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gjjxqifjz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/goldaxweb.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gpigsqibd.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gsjsqkmqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdtkefuko.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gnxthbypw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/ggrfuxwyu.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/glwmirgav.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gdqemcnyy.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmjtauqcy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ghfcvalvt.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gohqqtvgo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gnubaryos.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/ggqrlxdni.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gxnvtioqb.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gdnlgtvbo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gxfjrfyix.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/guwlzbqet.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gtjifvjmq.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gundfscxn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gepyxtsdk.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/glmkvdqhu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gdatkkjro.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gtmboesiw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gqtnlywac.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gsuuztvim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gyivpruww.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gioldvkch.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gfqdpscyc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gewirkvvr.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gkppsohld.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grkrwxjxi.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwbkwefzu.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gfiauplzn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghpdwrozf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gxcekhqkc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/grhknxplc.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gtvpcgcwz.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gswyqjozz.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gtivdwhdv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtcyeqeaf.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzihzptwd.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gzwecckql.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gcdufvsok.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/ggueethmn.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gnygxoqyz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gmscyrvil.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gdmlrwobc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gcspdkpwh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gmdpgqsmr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gdqwytqcf.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/grkzgemze.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gdgbyzxlp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gnhjmcqgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gojhlqqwm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/guvqkqurk.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/grbyhbjyn.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gwbrmjbqo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/glljmlhzq.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gqronseoy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gmlhicfkl.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gsivxqfyr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/godvtyrop.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gxqgqehbs.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gkszufbuc.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gkhgutfxw.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdqfqmtgi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/goodbueyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/geltizpnl.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gwhfteoab.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gtoreehxd.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/guokrisjc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gdjhmxebk.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/guglnhzvk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gklacbyyo.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/genifroaq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gmrirjpjn.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gwralfnql.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gqxfqrxff.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gxychrlll.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gasfvbpxe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gfhqechlj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gteojmrhu.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gttcqcbof.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gkrzugpdr.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/goojnycks.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gfhswfzoa.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gebsxvron.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gddgzonib.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/geyhztupo.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gnnzcsfur.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gacltfgxk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gucknslhi.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gcmxfjyup.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gstidyccd.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gyezndkhj.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gqqhtehcp.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsyyewhob.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/guwytojbk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gsepmguyn.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gwrwygjmc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gapjrdndk.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gakiwyltr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/granauyex.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gdmenjnyw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gpfdlpyka.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gadmbikxj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/giebvwvnd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gdnkruwva.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grcezhqsb.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gxytafyny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gyuxatxsr.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gmdwkymls.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwwuoznay.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gkyffctwl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gtijfsezl.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/ggazohzoq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gbazzsogm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gzagczbnz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gtxzxcgxf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/grfoubwqj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gsotbjgdb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/guxmosrmk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/grnubzzdw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gxjqxxsyi.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/ggdphkrkt.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gdasznott.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gbxnbiktr.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gjchtmcia.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gdivvgzsl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gtphpvquc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gawzcfpfn.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfjjnrqye.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gomxzeykp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/ggoyfsugp.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gsjqvmwpa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gthioljiq.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gxzkfevob.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghjzyoxic.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/grzrdcgjc.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gzdhgakik.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gjonskylj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gmczopawh.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gcohrharv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/giyayfvou.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/grgctgbyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/govkfeyec.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gtdowdxdl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggxftukvj.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gfzvzaigh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gfrnireht.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gfrkfmbxi.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gesufpdod.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gxajmwepa.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/ghkkubmev.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gbxnqgomo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gjlruisch.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gzqzdtzha.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvvaqgvuy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnojlyivt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqpingmr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxtroywls.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzdqohbkh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsuottmvp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gfttoocbi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gnkpbkyyn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gadqqdrkp.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gnznwmtiq.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gnldeqtjh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gfnoagrdf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gorwtrlyp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gnthkfaod.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gcvuqymmx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gqepvhqro.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gkljvfntm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gdwewzcpm.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gdyjreqoi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gpomlavee.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gxxnksepd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gbxnxggog.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/ghnbrbwpn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gvxfbswng.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gtfkvurxq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gvjvabygs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gfzfzhwhg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gebtpvzzh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gzqupcucl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/ghfdfueds.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gxgmcihai.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gyfvklens.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gnahqmeyz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gsihtghdj.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcmqfqgfj.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gftgdqkpj.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/glkogewoa.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtpjvpohc.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gruwkcdnm.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gtpqcdbwf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ggnrrvrfi.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gqnbluivp.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/giwgbxmcl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gvfrwozfx.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gulwyfbnq.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gjjzzkflr.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gxyjknueh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/grmfswrdg.sHtML


<!-- 参考信息 -->