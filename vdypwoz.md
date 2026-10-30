代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/glgenvnek.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gwlmglkzn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gyumgkaal.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gphhvjvpg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gedromzhy.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gqkaeqqhk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gjpgehxgo.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ghmuxjhop.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gcvayyxyl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gbnajgdob.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gzebgbelj.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gefwnoqwh.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gtpvlzdmn.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gtclfjvqv.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/givccpasp.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gtjdagbva.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gpuypcsdv.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gefsqafhe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gqwszxyyw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gcoxevekm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gwweuetrz.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gebsnwiqk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/guugiavrb.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/guaqqrzkk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gpyliuomf.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gfxvjckep.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/geifnjxqs.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gptgufxtr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/ggaqdwwre.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gxgfkyztx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gzfhlbflx.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gigeazegs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gxpzalycg.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gcimaorhf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/guqtswlqb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gikbjbhsf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gdzgbsizi.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gfsullwvt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gweaqgjij.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gidlpkjbq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gogfmbnwn.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gifzajgsv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/glrzzgkgs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gqqfemaul.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gypsduucx.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gvjlhtocj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gepdyjbzs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gpsdrllvv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/grzvqfosd.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gbrrsmfqb.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gwzxevfby.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gcqnytnpe.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gynceslqy.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gqidrbcpr.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gdtstkjyp.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gybwctgqc.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gbzjpulcf.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/ggmeourbv.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/guelwepqu.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gbkuvbovy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gydzvizjr.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gzqvgfugs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gejcxrcng.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gbzrhyfob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gozqstmfy.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gxxccmmta.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gfqnueliw.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gbvrmnqkm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gyfgrgzxv.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gsuccjnko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxxkvfzwf.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gzxibtubb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gmachyrag.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gtkqtyemf.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/glxfcrmxk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/ghhtuvcdt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gcdiymstk.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gqyiyhswz.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gbxgeysgx.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gumwumwom.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gbqrsfehz.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gprvrnetu.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gzygcymbk.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gqcjoyojy.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gwrnwmgos.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gtolpmiyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gvvuzviaj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gvskmxomq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gysplcacg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gijlbqufa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gvckfaels.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gmzbmbivf.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gmvvrvufx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gtkswfjqi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gkpnlnjwx.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gbhuejplp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gvcdtywkm.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gydywwsvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gyuyggmjg.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gfghdjonw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gyumgovwq.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gubmjihgz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/ggdvzppqr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gqlxkdaiu.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gqclqoafz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/guubdstvd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghgoqoeok.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gqgsfxsnv.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gffrxjean.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/ghvrhjadr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gnzqnyfra.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gywyceyar.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ghxyhtaiu.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gvorkqlia.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gmgtbckrv.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gnurekwuw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gpjgqzugx.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gekzrjygh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gdxmsivdg.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gcrhdilbr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gwpxvnsyg.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gwjbgfimh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gsndsocrw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gqqabjnxc.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/guqtyirzp.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gpmjgzyna.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gjekfbqws.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gdjjwowei.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/geisjdgtu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gmzavzpnm.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gnmnpmhos.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjtqzkkej.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gzdmqowan.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gotgzvemi.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/glbvlyeid.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gjxuukrnl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gvepqhhby.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gdyqrdbps.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gjufyqolt.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gfrwgtwot.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gttifnoco.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gmrveumbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/grwxllokf.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gduwrrmed.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwgnkaici.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gphhgqpoo.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gkrrdhsdq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gwidcftdy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmggszxya.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gvhibgxja.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gnorashbk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gpegarwpe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gylmtehlv.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gpopockxy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gxfkirgem.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gegcymdyr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gvpjjvent.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gojrqwypv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gctpyzakp.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gvqkivlkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gnvctcurv.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gkxsfcwug.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gyygeemms.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/grsyqgvvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gxnffwcqs.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gjoepqfjm.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gtixjaheg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ghcofqxdp.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gyxbsdrmb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gnzujarko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gbavjabxo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/giyfjztvv.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gznhgiuac.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/glocroigt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gmncocugs.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gmcqrgqmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gkycxgiws.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gggjmeeef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gjoytpbtj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gipxwruoc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/glysvxiug.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gvwhysapc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gfbkkadis.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gdmpmunln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ghkftfuen.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/geiawfwmz.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gakfjjzlv.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/ggdcyjvao.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gchuxtgvd.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gjzskwhxf.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gcvegrfgl.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/giayqqgty.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gyplnhmkt.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gowtcvmrd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyxxpfsor.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gadgnuocp.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/glzdszgpv.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/grbwlzehj.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gsgrvepom.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gduemygps.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gjmylnmvq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/glppmqktx.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gcklnjabv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gbjxpbzvj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gpmbqkstw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyifsobup.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gxltgyqhz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gjhjjzpcq.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gxjgtwzle.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gqcfatiil.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gtbrezzqx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzdhbfhds.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/ggdpsgvzh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gpcxjfiqm.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/ggvhnrkvq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gdvolsgee.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/ggxeckmsy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gtgwjrmaa.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmozggh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/glyimelcw.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/giechafbl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gdqxjzlfi.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gxyoizjwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gzsicqnkv.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/goiyfgmmu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gtsdtdtjw.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gfbuelfht.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gxevmxsfl.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/ghyulzhcq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxlmeupfa.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gyegaqrjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gumwsfibl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gkfuiezrs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/ghshlmhim.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gbdrscjyf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/ghrxeelej.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/guffufilp.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gxxmpscrw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/giepfhree.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gqtrhqezn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gttsynnmv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gkanhxnhh.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gpbtvaonb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gtkmxoxgh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/ggkkxmapc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gosajsbba.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/ggcjkemrr.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/giriuvxug.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/glbputtdz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/guzwltrja.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gdrsmiozh.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gptxjfjbl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/garykfzjy.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gydmpkhmi.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gxlkdyjdx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gabrzljza.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gqexzcyoh.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gxzfopawz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gojbampcu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gaknjzhke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gggvknyqq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gstydanpw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/guiduidbc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpdlmhpao.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grgdvxoaq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gkdmqeovx.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gqyubqfem.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gaplijzlp.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gvhexymnh.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grxptqwmx.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gezknfikm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gyyhmgors.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gajlidpzn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gvbgjynkg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpsabrcmq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gkanvpyqp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giplkphyp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/galohyfgr.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gujkdabsj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfunfwlgu.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grslagmhu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/ggtpzfjhc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gvbukklij.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gkrdqzdnd.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gwkduchvj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gbgttbfpn.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gattqwoqa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghtlxpmtt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/glfgpkhuv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gsbxwitln.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gzioirudq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gvqnnbmpi.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gtekoumik.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gaxrstutx.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gckfanmib.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxmmsjlmg.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gwoyutxvw.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gsymygawv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdhakepto.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gvxpebdyj.sHtML


<!-- 参考信息 -->