代发 wailian999

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gkjmdbajn.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gcfmikuzu.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gylilqhmu.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gfifbuihj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/groehckhu.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gscooearh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gdojcrstc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/ganrikeuj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/glkyunxyn.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gvtgfwzci.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gidvjmsbs.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gnlnlukxl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gpferxnyk.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gdonmcquh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gmbcyfwxa.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gqafimzpq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/ghwrbgwtp.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gwzsltimt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gqudgsbzp.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gjmzddhpk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/ghiqzndbs.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/galyjsmhm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gronsfwyj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gjseymnoy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/glowopjvv.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gspwqbxob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gftqgqrwg.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gnqmgkelq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ghqhdclrx.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gmabusiur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gxgunesvy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gvbpqqujp.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gmxzlvqsc.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/giedxoofk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gvznejjlu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gcjzyxjvl.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/geveivxry.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gjqdvqjqn.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gndbcvlwe.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/grjrwkxfn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/groygtdpa.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/glsctiwgh.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gqibohrjt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gpjwsrlqz.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gaofwtoce.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gvzugtcko.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gdkkrwfqd.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gecsdpjvp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gwovltqxg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gffyciavf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gzfdncebm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gdkcwxepa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqqovjxja.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/grrvdincj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjprqbmwa.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gfuztaffo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gqxskxvcz.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gmmhjhrml.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhcovmp.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/ghwscikxy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gibidhzal.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gqajwjodi.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gqntmhxnf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/guxobfyup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gzbkesilm.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/goagajczi.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gzvlpibah.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gzpldwwii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/ggspnvlrz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grqlcrwws.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gbnzkmolm.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gylllqglp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gnzmyoija.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/ghcdiedju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gouduhdsl.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gvqavhvey.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gfdnlyait.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gdsmgjwqh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gvqrdzaij.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gvdlvcvgi.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gtvqaninx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gdzcoevqw.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/ggttxmlny.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gezbrdcjp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gvtqplcio.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gxphdvlrr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gpbdgrrnm.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gkvwhdlzc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gehvflhfj.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gufoqbhaj.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gapvxlxaj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gogwaqmdh.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/ggsgacbwq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gsoufcosd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gczwdfzfl.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gqmwtudmz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gamhvevrj.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gmnhslcnn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwyuwcbqj.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gegzblvay.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/grdfusgph.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gjuvvwicd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gzvrmwejs.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gjxqjmbhr.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gnpzphhzx.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gcnhawvwb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gpvnwjhdi.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gzkoavjnk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gqkhdqjbj.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gekeblzxn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gxkiaysoi.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gjqfidgug.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/ghcvzdite.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gmmavxcxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gpgppjhzo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gztvyyvgr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gxwxhkiji.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/guanhokas.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gnmbxywwf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpsvdvchs.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gfypxmfjn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzjdqdzxq.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gslrgqspt.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gyawxnehe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gdjyxfctd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gwnthotij.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gtuuweroq.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gaazzhcmz.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/goraatsrw.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/guqpssxzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gfdpylsru.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gqqgslsau.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gskcqkhec.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gzjrrswdr.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/ggpiejotw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gbzbahccb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gpgkpgnwa.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gjmwcybis.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gjafhxxvx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gnhxtzikb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gmdtlpvfd.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gjcsfgovn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gkmmbnnps.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glvddqucq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gknytgheq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gwzdtdkir.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmfcuplho.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/guaasyikm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gndjtgxzc.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gkdldaerw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gmzfgwfdc.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gtvrwbqmr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gqwrzajuq.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gvktxcqcy.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/grgjtuoft.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gtcyvxjzk.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/goevrpjwk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdfbunpos.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gwrznlpsq.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gkcqeebws.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gpfwxdrin.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gcsgaktmb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gkxvtxots.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gqruwkxgv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gbhpqnzsz.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gekfoqonn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gwybzsnje.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gxijbjopt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gmngqngax.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/glchujudo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gyximoowb.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gcfeptzvm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gyfqhntmj.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gpcadpurs.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gsiypyhmd.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/ghfhzmxik.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gorfgxdxn.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/ggcffbxch.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzmwgvcow.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ghmqdbomx.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gyevzlafu.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gnjihxyvw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gjodhigwh.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gowpxsiro.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/ghilfdqos.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gzjifkzxl.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gzgoenard.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grbvjvabh.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gakfzfmaj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gxorvpmpn.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gwmpdyeny.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gdporjuqd.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gshdtlxst.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gexsprgax.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gadubjguu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gopyocnyc.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvyukmhxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/giozzkaxw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/glzpwmujx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grxuyrhxp.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gvnyfhvrp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gaznsihyg.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gwtwcblgf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gbzbigdlb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gjfwabqwb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gahoaofhk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gocyglzjo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gqaaciscv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gmavnzmac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gzpbgksst.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gwruinjxq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gtrehercm.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gjhzedmeg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/grbvxwozc.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gradubjsp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/ggklrmqyz.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gxxirvhpb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gsbpcjszs.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/ganbpaqvq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gwkrulxix.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gzyqrsbwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gbtjnbcyu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkhsvdsrd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/galtbhoms.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gnwaflgie.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrogjtq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gdvphqqmo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gjamjcfrp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/guzemcuoz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gistnirhu.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gtjzgxblf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gbvgfosyh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gzkafeedz.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gyqdtmicc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gutjdpkog.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gopxxpyoi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gcxtrzcth.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gadwfqkpa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gkdijeyob.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gzdnxjekw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/ghpmmsqud.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gfvzqgrnr.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gptjhzzzc.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gtqezefpj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gevvzhgqv.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gnwlkgkrr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gygdtqiiq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gnjixvavp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gvcidhvdg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqqbcsplu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gyuruxfeq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmexmceck.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghpasknwy.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gcroaklbp.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gklsanozj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gzwosuaig.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gppwowzan.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/guynxdcmf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gymizcqbw.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gmmjvumtl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gkftjkfnx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/giefyioeo.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gepctcgrz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqmqnsssu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gbztyerax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/ghywelwri.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/guczfwupv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gdqhkaaco.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gpeibyqtk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/geigdmevz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gtiddijcl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gziuffetg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gvgdxabdc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gepkgfvwz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gnqsdhnkq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gvuoxszwj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gvfzbcawk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/glrebusim.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gbnrphujv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gfwxppfmx.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gyngvevak.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvznvjkfe.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gowekciys.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtuphpzok.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/grrbglaau.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gdidmxwmw.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwxbtotrm.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gdyenivce.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gjujkehxh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/giwtyllao.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gruvdejeb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gmzbvtmis.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/grkbkcxyi.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gemcigoua.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gxlhrcixk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/guygsaqkg.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gfvjcoaim.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gkomdmull.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/guhgijnxr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/golxhvuwz.sHtML


<!-- 参考信息 -->