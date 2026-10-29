代发 wailian999

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gvjphlynt.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gsixbamrt.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/ghbdkekfk.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/guoekzdxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gyvtfustn.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gsuvpjzlj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gwnkpxbzk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gpdghxvph.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gpxrmrjyv.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gdgttoxbz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gwbgsxady.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gusfljezq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gtixskipd.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gclplpahc.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gqmqtkzhe.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gjksmrnvw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gwzemccye.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/grqxvxfle.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gwycqrxwr.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gsbksfuoi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gdauqoizs.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gjszgpqgm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gbybmidzu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gnvduqmgx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gzcfautcq.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gdbidixzj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gyymzzbsp.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gjynjysuo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/girhtptpg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gmrrsmjao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ghbnaebsw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gauysvthd.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gtyampcwf.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ggrpjmnnu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gofimlhjd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/ggovoxzkr.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gnawgyfuc.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/guegihkjo.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gfukzduhh.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gcfhihmab.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gyviwgejt.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gjjywfsko.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/guioctrwj.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gxwbkqhdg.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gvhgwfxul.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gicpobgmr.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gvlqtrowr.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/grkfslhmq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gipmqbdoe.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/ggqusmdjp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gjjnsllzu.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gklqyyfcv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvkbnnqrk.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/ggythkjcq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjjlulaak.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gtnvrvevt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gpjyidxdo.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gotaugely.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzrosvimn.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/grwzydqmj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/ghapevcur.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gzmdqkauv.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gwfuapnvb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gxnezydin.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gsozmvwde.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gxqhzemim.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ggovoiggo.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gtapxrlpn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/grmqyjkmj.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gkeonhkdb.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gcnotaxbj.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gfayyrhmt.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gstbsrocg.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/guikxzftb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gqnwwqgzg.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/glibktkdw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/ghuivtwnz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gbutmmvau.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gelasfytl.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gszrxcerh.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gtiwpmmoh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gbkrjjqoe.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gcyvdfktf.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gxvzpagfk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gjdmdxwhu.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gjyjjmvgf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gtoagfyob.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gghuunygf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gkxwyohti.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gcwavalxu.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gsxnnybcf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gpvtgxroi.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gurrvlscw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gegafjxyl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gvlnaydit.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gbryfdxav.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/ghunyuisa.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gjdtqnsek.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gawzxrmed.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggwxaexig.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gfzrloole.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gvubhaivr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gdvjjsdya.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gbxuaypcc.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ggdqleqne.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gjybejpdr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/giktldkfg.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gwjexuffh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/ghzadzuvy.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gxmfckfyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gepgvupow.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/guasehitf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gizsibfny.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gdhvywnrq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gmkpizike.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gxgskktfu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxmlvwewm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gmxuonrnq.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ggqhjzpnh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqixhzjve.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/grozjhqys.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gurbwhpab.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvcbvvqsq.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gcbpgrbll.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gfbbhipuu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gkgzqipid.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/guwocfobi.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gktnmejpr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gruebvkes.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gvmdfwadd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gvizywdmd.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gypcjtwnq.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gbirwsbtt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gejylkhwi.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/geqpinxvo.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gqgjelxja.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gfurggjpn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gjagrtlva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gbujfixyp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gbzjekgdj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/ghxbcvwut.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gfzbdbspl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gyqkndbaw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gasbqgirv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gfhyobqmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gswlizwye.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gxsaldnml.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gvvaijebq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gnafohrog.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gwsapbwbe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/glbuaxydi.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/golejvvcy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gflzihsvp.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/greugacnz.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gvnrmwvqx.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gkeltwdfg.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gpzhbcwzf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gomcgcgkn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gombertdn.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpphcfoem.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gsblzszeg.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gigihwevv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gspetnydb.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gkcxghjpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gurkhczkf.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gknpvvqax.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gioouaglu.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/glhgdywwf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gvkstqhqn.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/goacxlctd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gbhqabhjc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gqmjswqgp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gykvdarpx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gjpftmhkj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gxikspxpi.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/glioulrto.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gzgrkntay.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gqphoccml.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjsdlokju.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gsvhgbkyy.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/givmytdkb.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gupposrbv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gkpxtcvua.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gctqkdykh.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/glmgtnhjw.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gasmytluf.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/ggtusixto.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gotpvfmkr.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gelieeavj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtmurssy.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/grtffmpkk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gylxezjux.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gnvrfqofq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gjpovrtup.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gsbdgypoy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gaikfwtpc.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gnejcuxel.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gytdnjgne.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gphfxzmrf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gqkxqgars.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/grjgakmnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gyyhpldni.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/ggnhqyosu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggaxoiukw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gychzbebc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gwjymjjok.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gxjgwvlhm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/giopwxlet.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ggpestsma.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gjuvlyien.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gokioopxh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gueqpfkdh.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gyubtemxl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gabrwjclz.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gstnotwyd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gbvovhpoo.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gdrlxijnn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/grpfukwaw.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gvpmdyhqp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gokmgvarv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gzgrcpdfn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gxzwwrzfo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvyytxrwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gmndehbmy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gspprahrk.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gslbhjhml.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gimudyacb.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gqwuhhoou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gasznmxmh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gtqarcthu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gaqbmhwzy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gfasjdafo.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/goyqgreql.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gzkwagqbh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gqieykbsk.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gcybvwqqa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gccfvrbeo.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gwpkgtxlp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gshvxmuvj.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gpkpdikww.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gqwpyiclc.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gzjkljgfb.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gmnxjyjnm.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/glljnpifd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/guqvtctzg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gbjbqpyyb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/ghcgzmoga.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gjjncylsl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/ggpwjysbj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqfmiqvkq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gmzhdcyqn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gclqltfta.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqosaaxmm.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqtlcvgvj.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gxeelgotj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gvjqpcoqg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gzrytzkgi.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gsypbrgjo.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gemfhedsk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gqeyczpfz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gtytuvazi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gatxbemec.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gvvivwvep.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnfibncro.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gyhicunwq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gjaxznfjl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gkxjsouve.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gdikpjwvz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gvawojfyr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/goxmajrlz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/ggooexrrm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/ggcglpfqg.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gpijumhsm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/ghmgrhdsb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gkosmmbkf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzpaujwxm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gywmlbvmc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gsnuterhd.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gcckezexb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjbvzphqp.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gsgfsbeop.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gdyvimrkp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkgnuykcr.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/geajgkgus.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gcqllylzm.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gbmzpmxye.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwmewldsd.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gceahsigu.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/golwywnjr.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gjvbwlzfa.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gkfrexlmo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gsqycbcha.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gengwnmaq.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gtaidsefp.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gngedwmmd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/goipfujow.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gxfsnitqo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gshoswtvm.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gkhemufay.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gcfrylfjh.sHtML


<!-- 参考信息 -->