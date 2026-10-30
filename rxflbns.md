代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmktglmxy.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjggqxmd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoqurwaq.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcijuhekb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxkabsvk.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxrmbuqq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggedfcmhf.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/geoeuskjc.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpwppzqnp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gtwvajmmg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqzletvw.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gahbbehyy.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmttndau.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gouybwbnc.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gboympijb.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwgokcnd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglfdnbki.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxovoqpkx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gduttnvxp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gdvvdetxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghqehknca.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxzybqsse.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorrjklaq.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gszrtqdgd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gtxdauxqn.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gysxpkrbf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gacymnvpv.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/guogcljkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giohhgpqx.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjezcvzbm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdejhvjjr.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclfwogta.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guedoypwa.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gegmlxtyu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/guuenhrdv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gtbzslivq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gjsrawaqo.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/goelzmdzl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzhsuodq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxklkqlr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gqjmjussv.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gudgvngmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxxrwrcu.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gssqrhifc.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztkmwpgc.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/grmcfntdu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxatgsavc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzrlagdd.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxeqknyl.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvouxjuq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiluruqq.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gyovafsin.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gikiffsqp.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gvccougfr.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxjiswke.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbfneomh.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gidscahcq.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/ggldszmjj.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/guhqwshql.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhgaujpz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrkoyrqo.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gkhjwigqv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdqhgviw.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gykmrjlbz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grdsiwpfm.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gabnwaqtw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geiozkhgb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtovajjmy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwgxnsmi.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuweqyjp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwveoulnw.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gjxuwavrk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gzbikymcw.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gasisuxcv.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalivhwr.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwehvhrk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grftqkorv.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gppkqqpvf.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtabtnewa.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gichhtkin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gaqnttmxa.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzcoktuog.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwopjxqsg.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gkduxhulw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/giihdnozv.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkeidnujn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gjwosdwng.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupepekxs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxaklgj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/glguwbbhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gryydkrcl.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtuzbcxcv.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyisnrmul.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gryenfwyw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gaxrhciix.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtyrcgnp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijxubddl.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyjceobr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdalxgrb.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyywscdk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdymbioaq.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdmzdnmq.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiasuzkf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxjghyzb.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphetlfop.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbfxcoss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkgaugb.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gqgrqvdpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfpiwkyo.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpmdxlns.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqqhhxzk.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxbzfccp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gixyxwsco.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gepciljgn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxgiictr.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiocyxcq.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gsjmbgucs.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtgtvyaa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsepezdyj.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gysnhveac.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjymauukt.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gotakzyqi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gcakddxmq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gifmlypyk.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gocfkkbhq.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gemtshrda.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwvuvlfd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqnivytk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyozomafn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqheyrbn.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeyhztch.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvdszlklg.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gnifatuzj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjlgjqr.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkopufgix.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gwfabxvgd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfznwljio.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/goybwkuem.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gcdymkjbj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gndllrlep.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvukagiqr.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiiyiovc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gqnffdkjm.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnpcnenfh.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gscwzfovd.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfadculer.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gilbsmlai.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gxotvumih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxjmecf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gonygrmcl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrdsnkjr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmhvnro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuvuylmr.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsguznbp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkqctyxv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmueckqr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gurbdgujx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/goxvezths.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhuojzn.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfpogyf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdskblax.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/giynlqfct.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gyyddglyq.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbxzdhbjv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqlaowwk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmtnjngw.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gwfamhxsa.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gicrisjnt.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwduajvdz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ghpistoax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrsebzfi.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaopjjgrs.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnripvgny.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwsxbjmms.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcoahxrt.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgijzhy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gusbawpyg.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gphvjuwue.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwrqjqdc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfggvfhw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrrumjnq.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiotqgxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyncqyngq.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvxxbar.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnffjlfca.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gcibyingv.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gjhfsuajv.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gexmslsfm.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwkwomnzz.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/guyapfsqp.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsaezklr.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gntmiduxy.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gedwpwcpu.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtrgkjosz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gqkoynzfi.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsxaeysk.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqotstzsf.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdanmhjla.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/geivawjvl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniluuzve.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gcqwqvomo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmphobgtc.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwutnyvs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gbpplwgfx.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gqovzkktb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvlceiqwp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gjzmubkep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqltkwtu.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gizlcdmzv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gipxwgedw.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpznutjp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gejujpzlj.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxhjizd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfxwzvzp.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvajltlba.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnhsmwrr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzdlbjywe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdtzlvprm.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gilufjhql.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grnbwntug.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbvdeqnsb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpljrhjjp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefnrktx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/glqebkpxf.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtcryvlu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ghyhmiwfl.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/godpymcqg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdkvckms.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzekwnyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghulyrsdr.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsfwxlgu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghtfngaqz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxfypdbp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzprhkhag.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gexotxmjf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjjyurfg.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdusvjkqq.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnohuwew.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/grgpmgjqs.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gbddrrqdu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwljhymb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvyqrsgu.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gerjtkdmu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwqpolng.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyfrvzbbz.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/ghypveyav.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gbdxxvzug.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxxxrduzg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddzmhbtd.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gbyeyfopx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejrggfca.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/giagoootx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbhndmwso.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrouhisp.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gjriddtht.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/glxxpebot.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gwgnrzhij.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunsaglxl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnascdqu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gopagbzzf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gnsrauuzk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqiokycq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gbnrqbwwc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gowxmkokp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjqlzkywp.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfgmzzmw.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gduntqjii.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gszsqfqfq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxwicolaq.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfzmhcrbb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/glfnezohj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuvexjns.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapgxtol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gnrtjtsyx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyejpxxl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkazugogc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhqygnbp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzyovzki.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gwnfwlemq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacezfwym.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/getzudhzj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gwlytyjnl.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glqqindyw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gkajfoqik.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/guyigfhlk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gplcnakrw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gnojudexb.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsqvmkrh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gafvtbgkc.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjijagznx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbuhdcrw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gflvhwnjl.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/ghlzkyalj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjremcbqf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstnzpidj.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjrppuzv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkwfgqxc.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gojcouxly.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gcjizzcii.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/guazxebal.sHtML


<!-- 参考信息 -->