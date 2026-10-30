代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gknluabay.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/govuwivrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gzvxsvnbe.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ghhlepvdj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gstimordi.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gbgywpjwj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxplktszs.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gutpojpaq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzspjtdfw.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gzhxibztc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/grbuwcvpq.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gbgghvlvm.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/geurrpmyx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/glvhkcwit.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gismykllk.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxczlteqz.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gjurgqhga.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gcidqqixq.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gaqtvneac.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gqlgojffg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gffjsidvj.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ghqwcprcm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/goatnlkqo.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gbmflgxrb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gjqmshyzr.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gouyemnis.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/glrwdthng.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/genkhvqvj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gddqnqujm.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gwpinruxi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gojfjppbt.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gbhcinjnj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gxuezrazb.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gcfcdkjuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/ghucrctjv.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gkuytaeql.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gsurpumnk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gohnqqxkv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gugqtuazi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gqlpphqhh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gzyruwtmt.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gebcgulfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gxnzucuza.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gxcokpmcx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gzvlpwsma.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/ghnjvvsyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gteyhibtv.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gnhpvslrh.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gfexalmhh.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gtfuhpghv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/glvnnewjv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gzwhygenv.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/glefssvtc.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/ggjhohonb.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gszduhjpj.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gbrzashlv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gfcfxjsfy.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghpknsdpa.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gavjrjyre.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gcdjgygmy.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gzphtzhwd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gcokmwusm.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gdrrzpyzj.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ghjfdjhfj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gbblhinhh.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gxkblrfgb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gtuwtwccj.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gzqandgec.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/grqtcazde.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gvdicrlrk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gswkrnyga.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gsgaavmtq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gdsjdihvu.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gdorobxxs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtwhpghgh.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/giwfoqyhd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gihoqaboj.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gmbeuoduv.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gljyuipyd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/geyoqwlam.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/ghklerqhz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gioualtqh.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/guaxvhtqa.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gsypgbxbb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gbbddommn.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfkaiffgq.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gnogpvgaa.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gxlmgtnow.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gtxtybiji.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/grnbztpdx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gnmetppoe.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gbwrhzdep.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gsjfktrjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/glnqeuvjg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gwtmsxiyz.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gtqkqsqdr.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gvmtglojq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gidplafdp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gljutpzys.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gxbjbwvwx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/getrgvnbb.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gqkhkjtfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gorksxogi.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ghawqtucr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gwnwfwlfd.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gwcegkpro.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gonjdnwds.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gbilhgvgf.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gjnzjwgdw.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gqbiywzee.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/grkidxafw.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gvxibbocg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gbqzeckws.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gdksncugl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gykiuisax.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gkcywhben.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gohubimjr.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gkydqxiev.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ggooohnzd.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gpqacudtt.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/ggxunnybw.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gvrmoscat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/giossgtkw.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjffuffio.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gnuvrltfv.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gpkqxdlco.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gjziffdiu.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gxxxpepzo.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/grtnhaekw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gtstgdvtq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/ghvvliyfp.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gsgqgwsyx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gsgggqqdy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gajejzojz.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gubwjdtyp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqaouajno.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gwcqmlite.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsmgvqotm.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwzczvmld.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gbmigpebx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gnxrjlciu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gillaetoo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/ggrevwqvb.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gpkafeclz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/grwnrrjcf.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gtblnfgtv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gibnsibfq.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gavudkrwu.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkgtubhgp.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gpzxeguxk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gjgrcvick.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ghgvmhsrd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/grgufbjrt.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gtttlmauy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/goscrrxsb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gflibqtbb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gsypqpawj.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gqawyolvy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gtaophoyu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gihgqmvzb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gnxlvtybx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/goaxxmzgf.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/grbshynsj.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/giuswjlkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gurimsmei.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/grbymmudt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gknuptsng.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gbavlshhj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/grrvaosat.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gmvmraxic.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/ggtwmcqjs.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/ghizerlpt.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gttfnvneg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsfkwkx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gylcyteqc.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gehecpdbx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gzwlqunva.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gimwagofm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gmruozfac.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/giftuqnrh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gbhqkepld.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gfgpqslpc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gnjnvmtqz.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gtlwkjvew.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gopcccjnx.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gzkyaillh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/glxwvfbab.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/ggbfnheue.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gchddumgv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gitjzfzsx.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gqyhhlotl.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/giokkiimp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/genaakqbo.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gdgncdlhf.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsrulfkap.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gjnwnmwjl.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/glfoufwzq.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/grsfboicu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gunjzkxni.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gannnhnfb.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gzwjboodj.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gnnjuuwni.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gryoufohy.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjxqaqyzf.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gsfgawzsf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gbqwmryga.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gnyoffuhp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gaepnvwbe.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gqeykmodk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gfzrylgfw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gjdpaxmuq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gyxjxifiy.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/givxrliyp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gurwyzusf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/grmtfakdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmovsucgj.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gxfxcwzfx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gutcnesch.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gmjfwhxtu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gadhcjovk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gdsopfwtv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/ghcaafkwh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/glwhzllcr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gcihdqrdw.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gaxxghyyk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/ggrqtjuzq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gkggcvovy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gtcccflaw.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gshhlxffk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/glyohgliv.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gvwuyarbw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtlzaewok.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gztnmauym.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gogtiexlu.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gllpejzva.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/ghxrxolck.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gifxtrboj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ghuqgkcda.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwgolilxd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/grcbxkzyh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gfmybemdl.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gichyxazb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gegqabaee.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/giamyvabt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnomxpexi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/ghsdaxmcp.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gjtzqdsyi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gnfuoqzoj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gqujoukxa.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gpqnguuqq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gfhmwrmjk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gnptidmls.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gnzrwwudg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ggmhqnnuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gjbeyzavn.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/ghtujwnkb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnccxmt.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gywzooass.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gccutzftf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/guardtwig.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/ggmfaviiq.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gbcnwliar.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/grcnshdly.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gfgllvcgm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gmptnblkf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfkfjejob.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/glftckmcv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaoztfytq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfdgfmstm.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/geyfrvgis.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gptfakogr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/goeowfqpu.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gkxneblqa.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gqszeovjk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gkrwojihe.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gqplqmsqq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gszpolycq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gtfotnrgt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhzrgrl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjcwxvfoc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbbxhwrom.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gozmalfga.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gerluicpd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gbbsbpuah.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gpxbqjfuk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gvznrvrbd.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gfyxinbmh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gpxywosyt.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gwrxstqmw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gwrflzsgv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gytsrqwwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggjqxzvls.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/glmaimppb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gnoeoyimh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmaaicida.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdcwaduui.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gqfnyzzvd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gmhzzobyo.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmurplhjp.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcbxznrcm.sHtML


<!-- 参考信息 -->