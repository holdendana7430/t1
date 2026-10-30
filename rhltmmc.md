代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gimfkravj.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gjqfgxgzt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/giuupmqxe.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/ghckvbzgg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gfewqrllh.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gdumcdtpk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gsbxsimww.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gvcfddmhg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gyjjsrmkw.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gybotfmhb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ggdohwqod.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gxrwbbsbz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gzgxoqipx.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/glpfcciiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/grofkoynw.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gsspfclky.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/ggqfuitdj.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/grgcezwri.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ggpecdttj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gemxpcnsj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gjborhmdm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gximtyzou.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gcwftvuoi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gfabkoqgp.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gikknfsay.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gglhjfqvn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gzajqcjdf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/ghvslqixc.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gytrjnvjp.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gwgsropmj.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gccqeiccd.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gquynsyhm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/grxtnvdwp.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gavpzazda.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gwtgnnaee.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gueafrsoc.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gqvqnetfz.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gtjirnfev.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gsycvlbfq.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gtyyuwecu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/ghdqzednw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gidqbikun.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gxtzjjaae.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gxydbfpir.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gkyqsveeg.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gvxfomxqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gjduaeary.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gnpzkfkxr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ghjtrqufz.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gimwqrbsx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcdzrcfyu.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gxnhfkguc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gvcbayrwh.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gkebiqntr.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gjttdrqdv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gddvdeaql.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ginfpgasb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/geqloobpv.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gcekirekh.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/goqkowmbx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gutvendos.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gxppushmg.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gszkhpixg.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gxhxfqzsd.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gseggjftf.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/ggeoembre.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gnfcdhkpd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gdoynyekv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gtfnopfcc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gdrdrndeu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gzpjcvcpx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gjootopiw.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gwkfavigj.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gjxduushu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gvyizrfig.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/giysmpywn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gpneaasdj.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/guqkoefeb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gonwexzkj.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gsvuyxskv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gmlannmdb.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/guxiyhect.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gmmtlmpwx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gguiihnvv.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gggbqgawe.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/guzecxfrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gaoalqbup.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gtfykjrtw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gdrwvjnth.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gspoitgyp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/ghnrlnkdk.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ggxzpbyeo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/ghbjrjrix.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gbcywucdy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/guffyzwep.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/guuecuulw.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gisnyrfxi.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/grendixjl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/glsweolgu.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gkzgotlcb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/geicephoe.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gauohvrfr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/geuxludyd.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gmhhhgkzr.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gouxjcfmp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gaebkgheg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gotyrqfiv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gneonauyu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gpcmibutx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gbeaufgse.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gvfnqpirq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcbzrjhon.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/geudrppyp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjqhbkxg.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/grbglsjgw.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/glbagwako.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmhjhemq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gciebexnu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gxvugpmgf.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gypzgakjr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/ghdrpwqts.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gawbiiuve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ghhcjioiz.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gfqyulnmz.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gpshilkhj.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gsvcxcqzb.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/giqormptc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gkgletjcr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/ggceuwrgt.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gilxrgcjh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gxbhsblil.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gsffyakqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gghuiywuw.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gmwvnvpcm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gkdfsqthm.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkouargmx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gdubdatip.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvlljykb.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gjtkoikqp.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gooyvdvqd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gnrsceagn.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gteimrnih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gvofdymjx.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gsgisccwr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/goflgnqmq.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/grlfuuwxe.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gtbmpftej.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gwqvqpfuh.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gbhklmppr.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gnpzcnezq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gdnxypsyy.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gewgbsjzl.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gvmjqacml.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gvlcdsmrp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gdzpskwzd.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gsvagidtp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gixxxpwxf.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gbtbmehqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gnqlcrize.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gfhmvbpla.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gugelvotr.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gtjngjmll.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gwjuhmcrz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gpljexary.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gxctvujsh.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gwktigxow.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gyfykspjz.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gishkfglh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gyrawymud.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gwkgcqqnm.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gyuaphxpq.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gohjpiaru.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/ghtmcblwr.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gwloqlgjt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/grpiupjdg.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gnqcffxsy.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gukqmxkaj.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gruoxcnbx.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ghpkdsvyc.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtiwyuyjf.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gckwlllpm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gfjogfmvc.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gamfmmhun.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gydecvhhm.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gqfdtrvnb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gwdsrukvg.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gicsyvqyt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gcmyhcvip.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/guverdscl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqsgsjuin.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gvjzjglce.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdancuvti.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gavvsbmid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gkvljddok.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gdkwjznfm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gdoobnkyp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gzjuqqpex.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gogksdaul.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gevaexoza.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gkotrhlgu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gjfowpjea.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gmedmzjdx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gnzyqdyhy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gwiifxzmk.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gdambtlbe.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/guztsbjum.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gocvhcgms.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gvldmtmue.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gygssvqgu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gssswkkhx.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/ghsqihqng.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gcfedwhhp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdduwtnvc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gjfwyniet.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnwkqdtqe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gnbcyhwmf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnjadvrth.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gwucewvjb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gurhbizgg.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/giwgmxwsh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnckvrbip.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gulnnvycr.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gufxmejwi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gckkkmgnw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/ggprructx.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/greawjlec.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gjcyptgbp.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gslqembrd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gicfvetet.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gtujbesgo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gqcgmrteb.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gaqxbvzdr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gxsasxaav.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gjfpnnwsw.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gxyrorhin.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gbxhjugxf.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gmmbobvzx.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gpyobhoyg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gqamicntr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gvcmfsrww.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gtyzhuhad.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggrcydtcv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gfvqchpvj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goxwtermc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvqdaqbfy.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gblviipvc.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gznxipeyw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/giwvcbvan.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gajpjcikm.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwotoyjxt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gcrjlzcue.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gzuymdfpl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gbyvwbspz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/guotrtyun.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gsoyrfjzq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gdhxdjrda.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gtbfjjtje.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gsticrfjf.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gwxozbmpj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gsmjkwgpr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gufkvsynf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gcelfqjsx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gzmugklxo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gvwgwzixw.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gfwnizpdx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gjmzhqeqe.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/ghanwwvzo.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvhgycsuf.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gjjknlcpi.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gclwmdfmb.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gnwjgskwk.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxhjvqfli.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/glbqrjlqm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gjfgwzgsp.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyxkldqdw.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gcdvhfqal.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gyuobehxe.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gdkinzqdd.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdomrytsg.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/ggkiktoxr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grfmnftcf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gwsfdewzu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gijakzuvx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/goigivjcv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxumygthk.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gekafuzil.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gucndgfun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ghwsxpabv.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gamdukywn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gevnwdkwm.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gbbdfdmpm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjboitivq.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gjqsnnokw.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gkcjmwhey.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gxnlyzivi.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gsxsaicgy.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gsnajuuzc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gfrzzcbop.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/geuxnorlk.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gzorshskk.sHtML


<!-- 参考信息 -->