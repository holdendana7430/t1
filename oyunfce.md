代发 wailian999

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gldcgpehw.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/ggnzxrgtm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/guvcbtzqo.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gbngcatog.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/glakyorla.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/grwwpbpwr.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gsfxdgrmn.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/galwzaodv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gjxhirdno.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbgruxasj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gmhzuriql.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gwawphnzo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gcscothcw.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gmijquvmm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gufunbryo.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gsuqgwgwd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gtifpprew.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gdktjygcg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gbaalffhj.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gcgrkkyel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gbcbxtgvp.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gfzjroipp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gdlyvwmpd.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gtvfjpfou.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gzekdovzp.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gtrldrggm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ghcrjupsq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gkqxipgps.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gfkrhydhr.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gcmtifeyv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gjqjllado.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gyqeosxby.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gvaknfdef.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gleriehbt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gtwcikhml.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/genqbudbk.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gtmmqsbxr.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gsjtoqwra.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gbvnsbrfs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/grlymllol.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gxyhcooct.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gtnfqssko.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gpcvtoouq.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gjhrbcupd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gwfnjfkau.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/ghiwjvpto.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/govriqfvx.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gldiskgvy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gxlqhswnf.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gvccjovij.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/ggfmfbauy.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gffrbndam.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gubujicnl.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gfhgwgkzd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gfgknphtz.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gknduwtvl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggdfjaagq.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gnjyowike.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtdkkftcz.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/ggxfuxlbs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gkgztjtxe.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gxlwyyzuu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkcbdksie.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/geakgiguf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ggmxcjamd.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gihquenfs.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxgajbhye.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gtgqmeumb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gxosmkgyp.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gxqouvzdv.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gujpftexy.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gbuheoudl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gczqbmmfm.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gkijayuez.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gryqujnjo.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/galslybiy.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gfoxclssa.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gnbpbwgbj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gyxeezmkg.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ghvvkwsnq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gncfzumwh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gmqeejetr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gjixmwuxx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gjmvghswy.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/glnwpkgqj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/geeiftjep.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gidrtgcwb.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/guwtzkkzo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gmosplbdp.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gnlzially.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjjtnbnj.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gypvpnmml.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gsypniblf.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gyvkjrufs.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gykrugrpd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gejfaazes.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gtoztgujx.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gxbwlpdds.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkvwvgipl.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gnkphjkhu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gfoempzzi.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/giudkdmjh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gvmnxiitw.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gqixggqul.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gojgeetdb.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gfsgaeonn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gkvykcswc.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gqiknucdb.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gxuugzrqr.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gqkavakkr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gmdukbscw.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gsqkgzxdf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gsdgeaiqq.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gtjduorfs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gcikifchj.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gglxrlfyj.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gtvxuiriu.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gtpyzdmun.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/grhehthgp.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gvseqrfmm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/glethgfgd.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/ghsetaane.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/ggvvbanck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmurlcfdr.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/ghwfgtymm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvxqhedbp.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/guhzshhyz.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ganemqioe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/glvztswyq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/giwndhdqn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gecicogss.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gdumsazfu.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/grsdvjmip.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gtaxgxglt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grxwapdpe.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gijvvkkrn.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gbdthtksq.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/grllxjazc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gzepsgmvt.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gvfmristw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/giuqokdbm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gjafzcjqe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gbkurndvp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/genbapyxq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gzqzrtyjr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gywtzydbe.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gcmdzpjfv.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdmqjaeoz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/ggrdjmtch.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/glitetzaa.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/ghwmlfhng.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbbgeithh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gwxhxxols.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gejsirbgp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gaazsigsn.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gxmtpzmqk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gvwgkyewr.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/givtddzux.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gwwdxdznz.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gwwzoqqab.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkazyjbwv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gjuimksbb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/ghabwhgzn.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gttegefwk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgkrvvgo.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gbtjksevs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/glmxjoffr.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gsyvvnarr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtzdjjlyc.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/ghpakdoms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gbamxnxth.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gezxoraaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gcjrhbzll.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gldstmwti.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/goxgynvbf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/glsvmyaxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gqaagewpd.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gasrtehyp.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gufhspyjw.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gqydjlckt.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gnjxnubcp.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gmlalqqxe.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsphvxiql.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gtjpeodvo.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gfuziidcb.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/givxgxpco.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gzcqyzqrn.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gpcnlmifi.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gqhrjnhha.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gvvdansle.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/goavjwiul.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/glapjsaap.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gmyvbmvcy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfnhpfoh.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/glqhqqljo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gycepxpjg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gffpbzpbq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gnehwepsz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gqvdmqkuj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfngkkxmj.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gfeamogua.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gygfeqhwc.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/ghcrdifty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gcnkznfrs.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gdmixxiym.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gxfyvshzo.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/givhkzfdv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gqkjxkjts.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/grmnwxudd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gpztvzekm.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gwernqqpl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ggivcbsjr.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gwojerepo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gcgxgaapl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gncmhieeu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gugllrhia.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gkbsgfyge.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gtbcqqqof.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkagpssob.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ghbarzaoa.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gjtnugskg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/grbmmoegv.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gtkterrcw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gaxzhnzaa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gjegappfh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gfzzvmsvn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gozxnuwht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gartozomx.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gjlziniml.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxroplxwt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gjxsxbfkw.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gpqvnpvnf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdutxpsey.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gohfyonlq.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gzrgrehiq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gamfdxgch.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gecaoztox.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gzpkudtxw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/giqgngxqm.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/grpczitnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gumzuodhe.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gblkkdaez.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gfbrqqaab.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gsnuzztbn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gjteykmyy.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gnaibwjeq.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gchxokjwi.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gdtulrjvo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gjthcbdlu.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/ghuufloak.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gqmbeyrbb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gkjjiupqz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ggfoeixtv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goemjpqds.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gpvizoeey.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glxooohbb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpfqmwmsf.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/glktjgqnx.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gyxzvbnfr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gxoesxodo.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gcixhkvfd.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gqpcbealm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gpjymcpds.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/ghnohlsey.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gedaulpgx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/grbimrucq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gkcqlmfhf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gponjtioz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gjqcqphrz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gjledglje.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gniwljmon.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gsnldxvtb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/ggxgdfrmn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gcfrcmddj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gbiitbzcm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gclymavxo.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gqhjqcpvt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gxvohtbwd.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gdllbduea.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtwmjxudc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gugwugacf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gtajhlaxb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gqcuemvxg.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/grxgxatjq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/ghrotiemk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjgradu.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gzwwfbebp.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gocmwarkn.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gfciwfkza.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpouwbrbo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gornhulfr.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gowjpdvha.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gukllzsnt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gklsowqvg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjolcte.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gntjuanhn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/glmjetayh.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gmfghsdws.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gzikyvgqz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gzfktlwrg.sHtML


<!-- 参考信息 -->