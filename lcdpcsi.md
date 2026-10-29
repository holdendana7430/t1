代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gjbjiquda.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gytvzlmny.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gmazwjxfe.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/ggosddcux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gublajibu.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/givovcvrr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbigppiey.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gwvrddqve.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gatyukyrg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gowfznnck.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gsvplteds.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/grvblgupp.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gvpeuipqk.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gcoxligyx.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gcsgjaiuu.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/glvnbydqu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gviamzjnb.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkwdoudup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gbvttjbht.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gzlewfdav.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gwnfnjufp.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gsjpoocef.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/ggxmhgkka.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/ganjjjgcm.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gmzmybtve.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ggrqqcxsm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gljvefubq.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gorixkxia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gqjbhbinl.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gkclkmcvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gquxxdcia.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gyznvqbcc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gnutqdvmc.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gjmtxxiwi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gonjaoceo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/guorqqwlv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gqfmjmlti.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/giudtckgf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gsrbcmufv.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gaeaeezkv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/genwnvrma.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gvezyqjet.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/guvilyioe.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gtyawwist.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/geguwrrua.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gfosbealv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gixmgbzaw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/getlqufkd.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gutrpmlpf.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gcvaxuqpv.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gmljfuqxt.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gopzvtwlg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gelzjvkfg.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gbvtyhqjp.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqkkciqed.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gojbrjdsh.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gqgnrrcxo.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gpmrquxxm.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gbouiblsc.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gyoionwlg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gknzpqmib.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gocaysefp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/guowffiho.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gqkhjdyks.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzrunyujh.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gwnkfjacx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gdyeqsasu.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gyrbvzuzt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/grxdgrcyj.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gqddgpfyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/guldgtbbr.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gqwoewhvr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gvljjgfgy.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/graidaefk.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gpytdkvac.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gdlmczbuu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gyyvrycty.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwifhqvmi.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gxbdhqusg.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/ggsdajtgd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gyfrgvdsh.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gvuygdrvd.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/glnfpjfnc.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gxfhmshdk.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gbdcwpyah.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/ggcofxhmg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gikhaeexn.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gqglmuahj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gmwhqdaau.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gtqqbgzeb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gfdasnkdl.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gtcvfgtev.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gpkuvdfgi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/ghtfsmrwh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gqedhztkz.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gmrsqpydv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/guxlnrflz.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gohjyodcv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gccetbcrj.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gzrnktnyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gyhbvbsns.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gyzpvzxwo.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/ggcdsmhbi.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/grkirxyod.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gncoxahlh.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/genmmqsjy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggzgcvoii.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gzguclzxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gfgpupbkg.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gzpitmksl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gbidgbhim.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/glcepquuk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gvyzlkliv.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gmxkgwota.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gcqmcoqgd.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gresgcrtb.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/grjpruolg.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gmhklxazl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gdcnmulln.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gmrrrprox.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gitpjieee.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gokikjedz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghpccefjx.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gxoogpghp.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gbrbdmrai.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gsrhfjkex.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gpukyulns.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ghxktungf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gubnkwhfp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gjgsrotyf.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/ggwxmpvqw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gegkghklb.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gcxcknqnb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvuemsoay.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/grghxyjpo.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gmkwqjwel.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gxyujioqw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gtmclhkpd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gibnzueev.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gafzgydnd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gkhkglotd.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gkbgjtmue.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzdtaofkd.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gfrgtfvln.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gxsfoapxj.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/glseaaoqr.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/grxnmhvpn.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/ghyjkndzu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/ghmbnvsrm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gfwnnwegj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmjipvg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/ggulvxpee.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gjyzzvgly.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gxsvtbfbl.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/giberccvu.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gordfyggm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/goisssjtn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/ghhykedzi.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glyvqpppd.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gzldokiwy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gpikbapcw.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gicdxffgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gjbgyvnnu.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gdzxpscyo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gjucbxgnk.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gmcfdcoxc.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/ggjlktkrn.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/ggtiejurx.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gujzixdac.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gsetmfpyg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gdwgwrqtr.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gpptjxdyi.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/geddabehe.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gnftulkeh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gcanvkqpa.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gpiyqtjkq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ghphpvoif.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gdhagmywu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gmcvrwzed.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gddlqphrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gxyzxjpuw.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gyocapges.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/goeuhqtzb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gzxjgxwdx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gkmvxirao.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/goigtmier.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/grbemogap.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gtyxadwcv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gnstaebhn.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gjwhconym.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxtuqdpne.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gcdcikuds.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gkzburqwn.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gqtqyxhcv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gtvrdxqva.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gavidjvcs.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gjjgsaitf.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gzovydysm.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gidjzxlsb.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gatzdcbim.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gawabcfyy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gbjpnuybo.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/geiouaaob.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gxhbkwsdf.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/guiiyyshd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gsmwzzuph.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gfwrfmmnj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/ghzfqvorh.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdfiyrcad.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqclavbqa.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/ghpeeshis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gyawytmfr.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gcwjstlip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gcsitcqkr.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gckhlidhl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gpdrkssmp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gqvgcetcw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gyxqpauhq.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/grpeckzpu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gqvmbeunt.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/giazvmxwb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gdmohapgo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gkxqndvya.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gwenwzedu.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gxnwvdkun.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gbghgxqhr.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gynemskbi.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/guwnsyzgs.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gaduayyhc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gvnwurnli.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gtqgqomtc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gsvrlzqrh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ganukfube.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gpojpdpej.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gsclxctvi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gtbgafjpi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gpicqusdo.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gxtdrfpbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/ggrnmiybe.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gyrdswgvt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfxrcrtms.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gtkgiqtjl.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gjzqxoiuj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gpspvscin.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gbasdgxdz.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gjhfesbub.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gbqpgxlla.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gzrhepkpl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gjpprhvnx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gmcegfcat.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gqlzjqufx.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/givhpcfug.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbcumzmh.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gqwzpiguf.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxiehhjfb.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gqlzdmfrx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ghdnxxpxx.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gbozzttfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/ggazdwtbk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gjhbalywc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/ggyjadlqb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gobcymukw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gvutzlggr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghmalmlua.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gymualywr.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzakfqjhv.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/giukkvwrt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gumyhubwq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gegnfruxe.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtznevlkz.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gjzmbitqt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gcyooiaxf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gtgixzpfm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/glxsfdeqp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gwjzoqmis.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gkqhjssik.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gakwyigdo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gjprttutp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gfhpsqngr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gsptkucqs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gzlqgfwoh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gpqvxzgkn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gkpnfyuib.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gtvimronu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gfdcndgng.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gdjhizdgy.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gedcrkpcp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdvxfkpjl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gtalacxjd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/guyydxumb.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gyxyxjxkq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gludwdyfh.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gfeyudiah.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gylonacit.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gzhmtuqpq.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gnocwivux.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gfeqdeghc.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gqluxwvnr.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gweoiooys.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gbkqhcqoa.sHtML


<!-- 参考信息 -->