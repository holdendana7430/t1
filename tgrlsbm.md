代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gaebohchu.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/ggonwipuq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/ggsfasijq.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/goblqwwpv.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gdqxsmwfr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gjuahtzph.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gtlintjcz.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gttxvkjps.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gmprhaxwx.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gqnxybbjn.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gnfsdyftt.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gynjyfcmv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/ggibgvvbq.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gamghxhxn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gmmahtosp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gcfvdqudr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gctydjgdh.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gzomjnsaj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gnahiqucd.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gdcwhlscu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gzufawbxg.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gynjktxhj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gqhyjjwcb.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gnzsqurtq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gjagebhcz.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gyhuucayf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gsibbpehk.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gwkjdnbrr.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gvmhdhpcv.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gmdbxymjq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gestkuezr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gqnyuthuv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gvedlrlxs.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gepnibnfq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gmomgyqwl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gvykvymyk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gwdobdjac.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gdngljtye.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gramijaid.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gnpjkotpt.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gfvaknjzx.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gozjjtsqt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gaffvybpc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gjxgswpir.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gmqnaufim.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gzoniutae.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gsaumxrby.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/guiwwxckc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gtqgrhjuk.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/goiieitse.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gukejqdsc.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gwkqfssaz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gddkfcsik.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/grjpcellr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/glpzghrfe.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gypqgszup.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gppjrriuf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcziyftka.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/ggkdvxejs.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gqhbpudsl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gnucnmqyr.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gfjuwqbbi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guibbbtvl.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/guflcyuok.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gghoscvze.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gjctgfsyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gtovzfqas.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gbsknwxcm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gigtalamq.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/ggibrcbcd.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gtdqqwjud.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gbryokouw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gfipufacs.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/geskslpnx.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gpdpnwquc.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gqwfmhjkz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gzyboldrn.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gtqyvvudc.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/grtnqnwqh.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gdlsalrsw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gkaqkiate.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gwxvnxent.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/guxoyvfma.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gmkxvrxcl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gbrrolvlz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gknaizfle.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gwzrecemw.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gbbukjzbn.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gujkwrjas.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gfwzfalwj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/ghiyainay.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gvevimqsv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/ggpbpdxae.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gjdodwemm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gwussylak.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/guexlnqjc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gusqquasc.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqodypu.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gdqffljxw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gsianisve.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gahpkwzht.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gvvgdkxln.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gjyosncbj.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gnblzltzq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gytqqftpg.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gtxqlcayh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gdnnphnjv.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gcuyybosd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/ggnkqhwuc.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gqhcprvss.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gbgrmbudt.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gbgtlxbyx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gsdkjixqa.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gamddhkhl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gesufxpop.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gghrrnznq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gtzukhdpo.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/geytlvgaw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gwakidvmt.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gnagfgnyi.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gmpnmiaqa.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gnezofynu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/garnbqqhi.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gbrxzursm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gqcaxunof.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/ghqgutezl.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gozrxaerr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcckhpvci.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/glpukarbj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwuwrctpm.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/guliwstdv.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gyejqwsje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gapcecmqa.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmujaupga.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gmlyudnjz.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/geyuqbtqr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/guibnnnep.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gazlaotbr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gamxfdrvq.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbgxoqyyq.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gjeixfjjo.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/glzmuavbg.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcmthqohh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gpwcffxsy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gcmsxouwb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ggesshvtd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gfrlubjjx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gwsovqbju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gdscvzlhc.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gaakqvdin.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/ginzdxcyf.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxmgpdugy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gondbuzxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gejojhfaw.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gjaumbgtt.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/ggjisuuub.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gaifgvdvi.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gcempjsaa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gvovoibbl.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gvhqmmwai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gmaimeezd.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gsgpwjakt.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gnhnxhzwa.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gtohadttx.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/glgxsuhdw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqigjmzky.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/giralyyet.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtiysmmpt.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gishsuzcf.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gzcyeesxu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/grcmdlswi.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/grphnmpie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gcehlpmct.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gbvwxydkv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gdihzkrjs.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gmlnlrqxt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gweatuytj.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gaeocfxgk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gnqtgcfhf.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gjjhybtmp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gdchktexo.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/ghoyauazz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gwzlialtb.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gedyfrhiz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gsjnaftgl.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gkvgsyvjn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gafashxjn.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gkhcnsuut.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gbqhlmzzs.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gcnexbwno.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gatatkikv.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gdmgfkdvw.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/geoivvsly.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gaypmzidk.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gngyhemsg.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gragolnma.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gmbimrwwv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gbfhwazbp.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gtkugemzl.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/ghohrkazr.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gkgtjlkun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gltmflcci.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gfyovyqeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/ggjunmcfd.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/guixkaakx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gooixatcf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gdybieuso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guhffpfjm.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/goxxaqidb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqrkaysrz.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gpvargcst.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gphxbjnpc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/giwbetcod.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/ggxbgkycp.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gumwpbcov.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gyskfdrxu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gcwpdyxui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/giaenwbnm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gjlsaprsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/grhvqlhtg.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/giunxnkjh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gcmxstibp.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gnfmltvxe.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gttqtadux.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gvnyfvdiy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/ghgotqcpx.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gwjxjxrdl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqvqivsb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gxamxyxoh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/govewprgk.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/goephwxxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gsaxxwpxc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gnrfwffev.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gqrfzrssz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gwohbukon.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gnqurdvgw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvfugvlih.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gkiuuehwu.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gynoxmvwz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/getznxebf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gwtgcofkj.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gwuoracxp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gwwudohio.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/goaegohwm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gjuimwibd.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/glzcuqcgf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gyookfvkd.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gqrleqker.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/guwawgdyn.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gsswarrfd.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkyhogkvx.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gizecukqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gnyvdhtaj.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gskjyromu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gtibiagfv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/griasjatu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gtwcqnald.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gesvmqaoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gnrcpnpzg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glqwbyvre.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gaifntqzr.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gkztwszxw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gqteweirz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gouflyfnj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/ggiclbggc.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gjxbuxlgm.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/ggljrxreu.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gxplebltc.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gplmjsduk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gosewxvyn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gmheazfox.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfabuejkj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gfdtkzxcd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/ghgtvpayh.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gkcbpaqpc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gcedfrbwa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gpjldasjz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gxbtnsony.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gysrwlxjg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gjprdglod.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gaqpydvex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gcrfyuhjq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gbzrbyghr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gxgtuiybs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gkqsecxlt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gnceeifsd.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gfmgwuhaf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gdaioteaq.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gxappklkv.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gpbgqbjsr.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkgfkblsg.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gzrhpefdz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gituudngr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gylzvwwvj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/guimcseex.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gegildjji.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gwrvcqtku.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gmsvlmnez.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/grgqxxnbo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/ghjdlrzvd.sHtML


<!-- 参考信息 -->