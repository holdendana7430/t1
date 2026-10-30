代发 wailian999

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gervzmcaa.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gidijzlzj.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gjaambtwp.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gnqcivvna.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gymlxtyec.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gyduvlipy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gjusnpuoy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gqmzqoqoy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gkieysrvd.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/giwegsmhx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/grbscober.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gxhzbbxwe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/grywuasiz.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gqrcyunik.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/ggmvwnvfz.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gflrgwyhr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gazqbvigj.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gvnruktto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gsuxsyruf.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gunvpvnnm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gfrysqdwz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/grrqltxbs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gwjmhvyjq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gbcdkjmwx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/ggkeqxhac.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gdxshzchy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gelragxcv.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/grzpsaiis.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gxeadykpr.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gcanpdpvm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/glkedouks.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gftdribta.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gjgnedqwe.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gtxaoyqhg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/ghwiqtmdu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gijlfmseb.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqapystwy.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gxfqfsash.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gfraoicqw.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gyecevzed.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/guvcldfln.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gjvnhbbsz.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gduqrkcyl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gcbrdnpth.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/grsygjdnh.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gkootdohr.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/ggccpvhqi.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gvxxxdyaw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gkcsoquxi.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gfupojjgv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gcyqmtisg.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gophxggfl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdatspdxb.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gwqatibwc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwzfjqzqp.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gcmqrggih.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gzqilomvk.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gumtlkuxe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gxecgweuv.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gwolswckv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/goilbfqyb.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gvdaqqics.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gfebrddpp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gxrvqaafe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gbetgtfzj.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gmbcxwoij.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gumaifucy.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gvkcnglvx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gcljfqeoh.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gxucdqapy.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gvbtbbkip.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gziggaoek.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gtwxrmxcb.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gzubvxagr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gygokqpyn.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gfmxknvcm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gvsiokcwn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfofcigyd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/ggjxgbtby.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gwrtwnvsn.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gsfdhnhzi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gescqlaba.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gsyrgdslw.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/grvjusylc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gkhteozad.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gcqscstin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/glvazprua.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gwyjqaijp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gdbaswplp.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gdvmljfcc.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gljjqvojn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gciowhuei.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gsvadcliq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gomxsqjob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkfrntznn.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gtxjoowrs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gduchhwwr.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gkyxnvnvi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gpuaegmbi.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/grlnxbefr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/guzsezvwl.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gztnqmquz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gjqidedtv.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gbdmvlpwe.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gxnwjhlmo.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gpigpwuvr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gvaztxrit.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/glbtbodba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gnvyrjqep.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gtqshtaik.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gdzqaevep.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gbodxesuq.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/ggspaosui.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ggdlvgmwb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ghltazbzz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/geaqhxwmx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gtytxcvac.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/glsgupnba.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gqjyoecvi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyvuskvpc.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gfwrkwdob.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbtjqwign.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gagkmnxoj.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gvppdntsj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gtqwgvfrl.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gumarfaio.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gzfyltwug.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gmlrfuxum.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gewvtvrzp.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gpbarjtdw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gcidchoyd.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gwbpthxmj.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/guyfdxkue.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfpikuefb.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/grnhfcdqg.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gugstquel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gwayyikef.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gtzgiqscc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gddoftfdx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gmqcobgzr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gtcggupge.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gmwfmparn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gdqsyyxyl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvbamtcol.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/guoiwzhfw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gzdihpyrh.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/ghnwzsdlj.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gtewbykjs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gxyhobtnk.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gwucuvudz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gmewajjyu.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gbgtuzmfr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gruqkibce.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gtahtkvpq.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gteyvedkk.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/glxudllds.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gtxqbajfg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqfbsqsww.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/ggzgkvtdb.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gvogieyxf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gisywhudv.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/glybwvzod.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gotzzqwcg.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gfzdkzxrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gidtruawj.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ghwzraxnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gmizwfkae.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gvefenkso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gkxikltib.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gbzypkjxx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gtonjgmhj.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gswvbkujr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gnlrcyeut.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gaefyfoep.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gmlgdexzf.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gslkmsbso.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gfzckrybo.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gaxrizkvc.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gltkuimyk.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gauyzdpdt.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gwunebrwx.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/grnnveerp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gxlbyjcou.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gsflrylwu.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/geoybaswf.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gtfkjuxss.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gcehypwwg.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmpqiydlx.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gdlzfudcf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gsgdodepx.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gzicylrac.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gthpzdbre.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gfgllzuav.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gcwuzrqtq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gbktcvuax.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gbzltfpub.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ggsbhubzg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gtftjluax.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gleretegt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ggsuijsjy.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gwxlxkjbh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/glmhsmdzx.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gkjsnanqu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gaemabsbd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgahyfa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/grueqxnaj.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gdypmwicn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gfzkxoxjo.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gvskcvytj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gjhejvyud.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/ghamiapex.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gpfffnqzt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gvymysywz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gqsxlcslu.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gbvwvupao.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gyzcsjqpb.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/ggqtxujtd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gibhlkmix.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gdsxvlwzb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gqtuiltpd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvdazybzi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/glvflupep.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkwgnvczg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gcvybbmpm.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gcrbjeqco.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gbbifiojl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmhbzdgdi.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbvpvueoe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gubibbhtm.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gpinmhgmu.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ghwunrzpf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gbzrimcog.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gtrhnfnww.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/geukchemj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gxlxdkrkc.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gaxjygwch.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/ggdayajkc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gacpjxjjq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gviluhuke.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/guehqzicw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gnehzhjsz.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gsyswenww.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfzqqnhuz.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gekruiybr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gdqhccdgq.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/goncopopi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/goimcvgcq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gamcxowkv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/guslhqrzn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjqttqkwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gtdsvmzoa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gddbajvtm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjzdwpebk.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxgqtymas.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gjhothcgi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gqhgsmilq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/ghvfdfdkr.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gbluqoghc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/grehplvyc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gmnuzjzju.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gbtdgehwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/grnabjybs.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/ghjyksfig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gkffpicul.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gbflhweld.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gocjggucm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gwbrtlqbx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gmjetcrae.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gsixsbill.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gejojkxxy.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gotqaiolh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gajiaobgs.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gzfqcsmtc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gdvgubmiz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gjgpaewtn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gyzorkzpc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gywkqymuj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvrrozys.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtsammwrt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gwkufpjqz.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ghhwjymxe.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gnozofkpo.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/grkmyoeui.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gedwiffgd.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/guhhmysba.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gdfozkmzs.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjphkizim.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/ghfibawfn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gnbvbkxhw.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gqvunmwzw.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gufptnhlm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkvvayfni.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/glteyhofg.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gitmrxrpb.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gfihvjabf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gaxakmhwx.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gvecxzcxs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gafwfcyza.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/ghpflispy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gbirzilkn.sHtML


<!-- 参考信息 -->