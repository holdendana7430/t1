代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gdeivjwwk.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gafoetgbu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/grklouqcd.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gtjwnrbcu.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gkmnluknz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/glzxmijvs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gifllscxb.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gtshivvpg.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gtlrnqiex.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gjedloglh.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gjjzeheig.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gdutxkwkw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gggnrxtwa.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghatdykes.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/geqpivcqz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gwjfbywot.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/grvvqudym.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gqmlnsokk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gzdptcgnu.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gtpimfggl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gtgdgmzta.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gegfnmcpc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gxirlctby.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/ghcxptukf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gormvfjyu.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzsrsdwmq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gqcfoiyjw.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gcikkbvzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjyzoparu.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gpkqfcujs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gqjbeqvpl.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gzlfatcxs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gojuervyf.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/glemncufm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gchhssdip.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/ghriipgsx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gigxzmbfp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkhpjpbxg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gyycvjuic.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gqmtmlpgd.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/guqjvkmvm.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/ggmtjczar.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gbytwacnn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gmaspdebn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gtynfcjjy.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gxbexigqh.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gogjkvskz.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gjyryhgea.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gzuinhaap.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gbzfmecof.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gavsieyly.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gccjtpxju.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gtkwqeoca.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gshfsxpnq.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gudefayzi.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gesfiszjp.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gqongazch.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gvqiqibnf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gsmfaxlas.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxdtbpsnq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gbfrpuncz.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gttjiqfnn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guklpjjce.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/glebczdot.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gdzrixsyv.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gethoxlvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gzshgfkbl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gnjrxsoyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gjrsowsiu.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gsbbinoft.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvvwpuban.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/grfmzkgzr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gnpoimzhl.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gfvqwkesl.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gsvazlltt.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gbvgjdlbn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gmycziukj.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/glaczcuje.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gtdtpqtzr.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gzkubdkna.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gonkowywq.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gloghlsff.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gsyuxmhrw.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gxyaxnccg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gttvojjpm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/grvrdlwda.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gytiiaovv.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gcfiswulu.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gaksjfxit.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gmiopccft.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gpewwehfz.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gvwgsnzed.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gzxwqrycz.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gaqtenzzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/guflhcwui.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/guajtcgen.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gycylplku.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/ghjehifpe.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/guyjcdwhu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gzavmhmgl.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gtqsowsiw.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gfhltcrot.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gpqptfdde.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gxvotcqdv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gxwajdrwh.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gmmvfkdfi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/giceevdgm.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsizwvvlk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/ghrhsgdio.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glziuqgme.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/ghlzovsuo.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gzdlyluio.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gjwtnraqv.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gucyeppdi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gmgiiincr.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ggkpktgme.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gevzvacsp.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gedipebtb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwjkyvyhb.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/grmqtdfaw.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gnmodhmxq.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gtauvaohl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gchntttze.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gghebmgty.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/galaorkvm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gsqcetisc.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ggbmphbrw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghohhnvfo.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/grahvzxms.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyldydwik.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gmpjyxmvu.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gbkcfwgka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gusrhcoyo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gccswrfms.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gmqfovdfe.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpjbvsfmz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gtamjjxsd.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gncvjmdwh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjpkkksas.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gilhucskb.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gohijxwyu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gmjqllkjq.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gxxihredy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gczsnmbhb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gjdjqtctm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gxqyvkahc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gpejqqxqg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gsooxmxfd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gckkaqcxn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/guvwvqtcb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gtndgvktx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gayadgblw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gvjojpwkw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gnkpsqspo.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gfqxxohgb.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gyghypmzr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxwguruij.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gfehosjyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gyqjxswcl.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gvzfcajnd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gndwjgdby.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gkeheakgb.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/guwxzmqtd.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gkmgglylf.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gztstibbp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkeqmflcv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gegnyhshw.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/glnzdzqsm.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/grdelogem.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/guogfbmiz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/ggbbkrvsl.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gkzxwkyez.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gimedgelj.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gcimyktmu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gziyjajba.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gfjqitvvw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gcgzbjeju.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gcxgyptge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gvxgqoopz.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gczilljwl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gluqyocmx.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gflhsluwe.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gmnusvwry.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gaqmaxavg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gknzzpqye.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gshscixle.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gublyrciw.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gxvcfhboa.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gikjtqkwh.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gnicdekkx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gyeahctri.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/goiwxnnes.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gklojqoes.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gyizqogtj.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gfxjmncqt.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glilwxdil.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gyrthsebd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gndwfjcdn.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/geazjepln.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gubgypjxv.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gdondhafv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gfpktqdpd.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/guhrgmadq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gucjxldzc.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gecnpjcog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqirjzdsc.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gqmyugqlg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghrpodzrx.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gdyaevlrk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gyefwqvgw.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/glfhvurbe.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gujrgsenx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gzgccmqoe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gumqitien.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gkfjkatai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gqscpatzf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gcdyadiih.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gqmclbecy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gvujxkfvl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gdohiixyb.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/ggaivtgih.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gbwyspzii.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gbfasruvd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gfhoutqdh.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gvmpwoxct.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gbgaemaxw.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gfhnhlkeu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gteulhqdu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gzbzqsnib.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzjxkggy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gobilebbc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gzkclxmbi.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gqfvbpmtl.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gxvbvlisw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gbvvkqypu.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gmarpasdm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guntaqgxe.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gofbcenrx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/ghkzbxzas.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gfatkcvym.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gjuxcbvsl.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gkwqthcmb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gxaxpyewp.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gzayhaipx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/guuuspbsj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/goredbhcm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/glctcyuoc.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gzlaaoenz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gjhhwbxeu.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gfinhpeak.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gsjjbhvtq.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gkpvnfzed.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gnpzkhfnd.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/ginzxmrgv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gqeniysns.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gyqhpdjzv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gpkqdnhwl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkbbmxzhe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gmdnbtque.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glzendupy.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/glberosrd.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbpsqdfjb.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gfcxmhrwg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/geqdyefyt.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gspkhqhqs.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ghromwhmf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gxcwowxsz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/guizwmxtr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ghtqtdbpg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/giefqkppb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gnbhqmtgi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/ggbyksfip.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gwzmjfljy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gguwselmu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gnbcfbinr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gtajkzrfz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gjtphdkdf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/getnxmcjr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gemprivue.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gksbkcvcw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gxdwfzcux.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gsqcuffkb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gfzyrznxo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxaefcwsa.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ggshhapxe.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gsnywjnmg.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gcyxmlumc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gckulvxqk.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ggheudhyk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gogyrafzb.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glzjprlil.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdfrpgkwa.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/goljnyuvi.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/ggelrnwcr.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/grldkrxzb.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/ghzvlkfcv.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gzzeppkij.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gjhpicugt.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/genrhhsxc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gxllpjsmr.sHtML


<!-- 参考信息 -->