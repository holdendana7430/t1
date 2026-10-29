代发 wailian999

esac
来源：http://baike.hesvh.cn/Article/details/gswrgkqmt.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gdchhdofb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gwmkpmnlw.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gkvumejqn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gjiziejqi.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/giofrljrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gawjbqitg.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqsfxldsy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gkeufjfsc.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gduuzckhp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gxuazhvmv.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gojhqqfzq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gtqssypda.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/ghmenwqqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gckmawrys.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gzuuckvxu.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gkzpydsbe.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gibrbsulh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghxkswtzn.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gybetuctu.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gipchjgsm.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gmhjeatur.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gsczkptgh.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gyzmmmmtm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gfvbswlrz.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gekmwqrco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/grzjbocvm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gkwyrxpys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gzilpumbi.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gfuwbtwqe.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gmkjzvrol.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gdlxhjmjz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gsqvyqyxq.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gvuuzxxvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gjvjmxgkl.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gzwrpsjkg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gfnyekpgy.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gwckfroya.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gtcxeteej.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gidmhexfd.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gvzfohjyd.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/glgfsrefo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gpsopktfz.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gbumxqsqk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/guunlbmwx.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gilfzprux.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gsonhcdxz.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gbofvlang.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gqrtyictf.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gnxhvujdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gjnkjvadv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gfzoitwpd.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gngcukhke.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gxctlccvj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gzeyxzezs.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gvjomikqz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gevyrkjsh.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/giljplgnq.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/geltyakrt.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gtvcaewir.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gsmqdaefy.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/grkbqbltx.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gqwspvvre.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gjfafkvrv.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/glgjbcmam.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gnmurfcgm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gpzatddom.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbkfvlbcw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gtrwrueot.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gxphcqpeu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gxpwvopnl.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ghvfppitn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggnhvejcp.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gddqblqah.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gxnejsprb.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gmcaokqvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/ghuwuzpcw.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gjxtskrjq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gehqnhbdz.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gfdvzyjnk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gdekmubxh.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/geyglqheh.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/ggimjuutk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gtmniosrf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gtcqqdvov.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gaqrzrwst.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnbexlget.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gsrtrtsxh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/grbnnqwdy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gfzelsgnu.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gummxzshg.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gvqtbrdsa.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gkrauutwe.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gbjsahkpz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gnfuqvlob.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/ghgypxxzh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/giflvpoyg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/ghrgawgtn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gmromulzy.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gfpirizgb.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gqnuyhsxq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gloxqniio.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gakhwwlrr.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/glptpvfwe.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gvpdkfdem.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/guqfzmiai.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/grhwirxxa.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ghzyytfej.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gmlwkrcgs.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gtrzmvxco.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gcjlddzdz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/goytgffvz.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gwbahovon.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/grlnjstuw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/grzatoibg.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gdaaucifc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gdcgwhfay.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gupsbdvve.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gfhemfwdb.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/givqtauag.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gisagywai.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/garwxjlhz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/galfukngu.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/giigtvhfq.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gudcnfmoo.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gxjzqowhe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gxwvaofev.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gpxjcelja.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/ghdbbnzwv.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gxhjbzetz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/grclleqpc.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/glrataahq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/grgkjcmnn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/ghxdgrthh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gpyamcdpx.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gujhczsvh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gklljteic.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gbppjehcg.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gegfssymh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbbewidma.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gptsfchoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gewkumsyr.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gutkwxros.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gdzpnaaxs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gcqdliyra.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gnnyrizwd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gdxwquspl.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gyhuibkty.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvospsqbk.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gwysohhtg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gxjyjjece.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gcqjfrrxx.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gunkpdyei.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/glguhxvbz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/ghjfmxgyt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gdludamyr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gzzmsiitq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gxkctwoph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gmmewppxf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gdenjuyck.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/guimkxvmc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gdogphups.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gohslihvp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gbbhbdvwy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gkqhhgfir.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gpqzuswwo.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gegtmsnrh.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/guymlnzsq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gafdnznwm.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gvqahengc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gmnidxsdh.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gzrzmjqel.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gbaqitgfa.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gutygcafr.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gfosixfdo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gtctuyrkm.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/goxccjorg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gvngtvhkj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gtzuksnpw.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gjlrnsyfm.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gkcmqevug.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gxhnzydty.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/glhokybql.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/guypbjtld.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gamjczral.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gbhotsguj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gpktomewv.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ginqyqrli.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gitgbevkr.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gzdjwprzp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/grrggpkfq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gxwzfkolf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gvlzruhhh.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/ghqkiirhs.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gylmmthva.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gxmihnpil.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gdsaubydv.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/giuwjqiaj.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjvvkwcdm.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gztxzqbxm.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gmuadgasm.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/glbwihnrz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gxwlusqcl.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gxkwaxbsc.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gxrholnyx.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gsiqodkpf.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gllsrvglc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyliplyfg.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gjvdmmpzx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/ghslenkqa.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/genwixlll.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/golsayeek.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gogsgkwfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gcogjklsi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/glehptovc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/giqemsvds.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gcclksean.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdlqywuln.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/ghojvsrmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gupwzcynb.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gwxluwfyh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gbvzjjrmj.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gpuxcbkvf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gzieobgtr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gdsqxcqvf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/giycopdef.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gizinnlkw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gyluyeirx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkpfcdsxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gsdgovxle.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/guaspbwzn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gddmomwkx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gwmgvrjlr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gswrthbwh.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gwcbltmvd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gyzdqamfm.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gbrdfuvjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gwwudppmb.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gvditlnge.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gjjawejra.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbmccnaws.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gzctnvncs.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtewzcdte.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/ggorfchct.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gyzfazuxb.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/ggdxgetfw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gwjebsvll.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gykhwqdrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/glwmnswmb.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjgsjwqkf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gyselvgex.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/glecsvzit.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gptriykdi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gtikkoryd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gnzyihbev.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gunbvpiok.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gfwtabqrp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gfgwcpfya.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gksxgzugw.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gctbgmllm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gzovdcztr.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gkrxhxaum.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gsiesdlxh.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gxykwdrat.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gryiydbqh.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gixifirmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gtxwzfzma.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/grayyulfm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvoqqzlel.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfkhvlmgi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/giflgmokc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gunqkwoki.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gozrwaknt.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gppmklfww.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ggqtsgvkk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gtpkuoffc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gysmghnow.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gxhcuzfvb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gwmlkvaon.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/giexstsue.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gfhttwgsz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvynbaeod.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/grekwiddv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/giwinkozw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gslyxwzsm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/goeyiaahb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gbwesllfn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gomxnjeji.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gukrgstua.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/ghabuehlo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/govkrmjjy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gifyojeoz.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gagbwerfs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/ghzthcava.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/glqfshcve.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gamqjlzdg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/govpbqpld.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gwljlluuf.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gxmzsilcg.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gebsvvsjj.sHtML


<!-- 参考信息 -->