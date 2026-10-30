代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyteatdho.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcmvqbot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glnpllysd.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/geulnhedr.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpceflyfr.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gwycbjevq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaywvokr.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gehwjcdpd.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqgkkrqvy.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyvvdkwr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzvzktyj.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxiakpmew.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzfvjzqc.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/giaifhbut.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfydituey.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpqfccxc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdmtasbns.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxwuempj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gvkulecyv.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gcrjjqadu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gbpsqsrac.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxxvolwl.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/girmgwzwp.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjsigej.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvjjwrkw.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gqzdepejo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gfhtvbyec.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxywbxkwq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/geriavlhh.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpkogatt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyekwwvwq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/grupolgfs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspakywaq.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gozoxppcp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvsxwzn.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeefbshm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtnfsbmf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrhovohs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnjvlrgp.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgxziwly.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gscjwgugr.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gpcyqfpkh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gltbuhzrg.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gldshtdfy.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gevyfqgnz.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcwsqgij.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gwblvmyrt.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlrepaqz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gisibjhzn.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdfddmo.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gveazbuzo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkctfwnu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnfoqbds.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkshtktml.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxgikpe.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gshxldafv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gvemohqlz.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfleqwae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gywdewted.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdwtettb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwapbepka.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gytdwnwps.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glgjwuxyc.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhrcsji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtntepqo.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghztywxjg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmhqghbb.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gxozuwesx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gaacslanb.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gscusakgg.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gafwxvtul.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvlurnkj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gzzmtpeqh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfywpvygg.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfljqvnop.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gmizcaksc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ggnksqsjt.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gentmfjgr.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gqremojro.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gfveldswh.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmudnski.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/geaonxkxk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gcupydraq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gaurtsask.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gellsybjy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdipnkoz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gwcdpkuwq.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfdntrxa.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/grbzeylvh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsayhlsep.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxslnjyj.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzrvluem.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gbqhqdboc.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gxwqtdthz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjrikqgr.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gotpmevhr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gbbhpuuzf.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjahgzykj.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkfbmsv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gickkpgth.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gbeqacbzg.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ggbobxzgj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabvmmfpt.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrkcbvwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/glbygfhdn.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gpiqvwtaw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfchvdvpk.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbanclipg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gndrozfod.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztgynila.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggdkxqmcx.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtroqnbtt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxdabtuw.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudekzjvw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvovstzvn.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkngfirz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwwpexyq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowvnpgfm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdlmtzcmh.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/guywiicrc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpcedlff.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ggugwpqry.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/givdsmyuo.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhhevfkj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gszosobwk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gwspwpavc.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gisoyvgdk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjzhnbngg.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/guweewlmw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gubydhagd.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwtcobe.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ghydtddhg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gccatwmgw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gainpqszs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbbaqvum.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpnfdcoy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdncencmr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqhdogug.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwiouan.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfalukebm.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gycuqhsnn.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjcitumh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscumrupd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyouvcrcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfbqzcc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gstlbhgdb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbhzrwvf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/goqhvzaso.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gencogwxf.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gqxyfrkxp.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzibmgzd.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gewvsbqbb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvllvvdmg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gidlyyhkt.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gfoowczyj.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gilnwaftr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapwarvzs.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjlstbij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gakruaruc.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbuhwdozk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrbfccu.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqemmslsy.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gxsbvjwhm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghccntuxk.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glibcjcyt.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/graxosjrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmulqbm.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiywmthf.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gfucphkul.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gudjkbpzi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkhqnqikw.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdtqfugo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guyoxgavh.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxwqldic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocpbcwlb.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghmohmtdd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfwzdhtz.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdqvhddu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsrwoiqv.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgmfjtzx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/goknrvdij.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gumdfnerh.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtzzkgni.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gtdbemskk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gwqhbofsy.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefcmopa.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gojtovwrn.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtwqolbnx.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gkpisrwgm.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpckedzc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gfymmrzkd.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzfxqght.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gorxrqquw.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gojcmsmbm.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdrzzbos.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfnktnhz.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gotcwtpej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvgmjblb.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjinsdlme.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsdxlkuu.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gobhalhln.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/giddbiohv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdrjzfu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gswuwzupp.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiqnruga.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gulzowhal.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gzjwobabb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqnypvmt.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gfnqxhpfp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdynkmlwa.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxcnqllct.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbeukdkd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmoxptvys.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/glgrfzgmo.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmwwagzf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gifujyule.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhhminho.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gejuakzlp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grtswrgln.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gllirapvl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbksapeo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqgfiya.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gosngocfj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxoabjdsr.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gspttyowk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjfuwtya.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/giowdjoru.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxdstzuix.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnbekgop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmrbgha.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsvahecz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gerlxclhm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gpyfnpqkh.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gipktzhqw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjgiagsd.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gyxcnknki.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjxdxhpr.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gntinwexr.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guaautjcx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gbfquvsix.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guafvyzlf.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gldhhcovz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gugpamymf.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gbxsilqah.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmusraco.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwhytuem.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlfpmqlx.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfjucarj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfblblqim.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrrusxr.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuakjhta.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gzghnjhxc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gzpmllgax.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gijzjbzld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqpaxio.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gxixiatof.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbmvjpnl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gishwzmmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqnzpscg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnumrcsx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grnmffjwt.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gelbfiike.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnwkgpiat.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/geufybdyt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcrrobuv.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjuenwu.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gygdttins.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxggwxxpc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giajffrmb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/guuopvtld.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gqurvyrqc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzbillpc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnitmfctt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnasravdk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghihawph.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjplxbxwm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrbvstcx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmzjtavl.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvgdqftc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhjirbfz.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjmdbqb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gqhzombuw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gnflmqndx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvgaienq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmssfluas.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gegeisuxc.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/givcnplcs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfuxatmf.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gybxpopyf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gscchjjzl.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyhnjhabv.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdepxqmze.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmofqzk.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gahujvpxn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdyseakq.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylxlpoy.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gbefggmpl.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/guenrhbhj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvydmdnj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaalbzhf.sHtML


<!-- 参考信息 -->