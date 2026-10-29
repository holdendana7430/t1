代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gsspettrh.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gfgdjzcfe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gabtdwxym.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gebfledei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gvjwbtzqn.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/ggbwhctdy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gitsxxegq.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gkwihmnqs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gzifiozlk.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gkepmqaox.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gqclhzkxy.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghhxcezpj.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gycdkzbek.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gnhsygxad.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjwifwmsc.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ggmizelud.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gbgjnozuu.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gatzfstld.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gszsxrzpv.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxwffozhe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gxopldqgf.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gyvchpldv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gsqqmhrgl.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gqvwupjkj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gtaxtrimq.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gcmgcqfqu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/grvtoynoy.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gkeophzku.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gxobcsjvw.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gjinosowi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gxvgvnvgj.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gercwojkp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmqsnrgoh.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gqmisfjjr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/geacpczdm.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gjswqxovq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gnuitguos.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gjwywbwqs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gzasxuvsi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gklxeeqch.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gvjzfqqnp.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gjbktqlkv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/glvvzaqwc.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gsgeikfdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/guzjhuphx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/ggmhvarbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gsnwsccwm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/genvlxzrj.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gkvejoyxl.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gxvmgedhf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gtwpnomuw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gcpiiwmps.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gntpvpwlu.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gmzkbdtnz.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gisvluokm.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gxvavqhdf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjguszyig.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gcsoxyybw.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gogaptqte.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/grepcimds.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gjrupfwdi.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gfayqdusj.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gdziehyla.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gjbhhtmuj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gpclvbrfn.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gmfvpafra.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gtffewrkt.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/glgeqpilf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/glyrowzdq.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gqvgoawtb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtaqjosdg.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gbnywnerp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gleuzsggm.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gwvpawahr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gllufzicr.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/goqoljhoe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gjswswodh.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gnxshcmhd.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gnivamypr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gyftglwci.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gjojcmjwx.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gfczovfig.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gvzcitfqr.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gixdsgsdf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gxgbsmtot.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gfmgdxdkg.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gkdalftjk.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/goyuhdvjg.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gllcvrdrt.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gupdeufrj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gsttcxpyt.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gwrmaknax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gcirpwkkc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gyujcvxtl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gkiretlod.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gaucgrjae.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gcezcyvsl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/ghytixdbi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/grluwhaaz.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gsiyzcxux.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gflpcxgnv.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ghgxfjmzk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gluapkvhw.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gbwqhwdtu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gqzqmvfli.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/geqhbuohj.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gvessadxz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gqrdjcyfo.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gjdueojuh.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gbqwhuiys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gokigjqec.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gdoeqxeuq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gixjchndd.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gcfbtpwyp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gldrzglud.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmlfbrlyc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gkgyhiooi.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gqzfxqxbv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gufqcvoit.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gowfiacbw.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gzxpicais.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/glfyqsiff.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gjsthcpka.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvqkhpthf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gezspnhvo.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gjchemsnm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gggiztzqz.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gjyhkfgnt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gcurrmseh.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gltmpheoo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/glpheozqv.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gldprbwxi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gqqpycegm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gegdzuhxz.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gvnuawbei.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gclzkwiao.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gughlcdkm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gllgywzfs.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzmkshmkj.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gkumrtaii.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/ghmgpqcnw.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gpckpfwsy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gibknnadp.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gpgmlkumi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gnksjngue.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gflvingnb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gefdtmvkh.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gttfnixkf.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxkudcdtl.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/genkckolz.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gicdhwlqz.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gpzgwerio.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gaznxrirk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gjyprkspc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/guzwvxhoe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gswgmonbq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gkyffchwc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gtcwgjrsd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/grakcuviu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfozufjyy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/glmkyrsgt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/giwlxwknw.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gwtrpvncm.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gckqcpkaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gavgiqofh.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gpcqmvtyo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gdeqqlvob.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjhyjiq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gjcjigizt.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gompkjzya.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gprfrpril.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gssnukcbg.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/ghkivwymr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gzbvkqxgu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gnoihrbun.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gsfegdxmk.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gikryihom.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gtejbskrl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/godgttbsk.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gtxzsswwx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gnsickktn.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/geilyiwve.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gznvlifkb.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gszldbsbz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gzinenwnh.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gmvgoyfxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gclvyzymv.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gimedpsxv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gdqdjossj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gsksnfcdo.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/guivrlehl.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gnbxacgzf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gjlzspzjy.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gvobwmlil.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gvsbkjasq.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/grcaddhfh.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gajjxyrrp.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/ghtwvbmvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gvmcyuplx.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gmwrqfley.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gtyyqymdu.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/guixxcsnv.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gdkugvere.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdydowvlw.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gwbqyhfdm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gqhxgksct.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gbjvazook.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpqcaatju.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gisrbmvbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gjfyizzhg.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gslslpsii.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gyxyounqb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ghbtzdlep.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gjhxgfldr.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gvxmpznzl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxsztmocd.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gcpiwhohz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwneejgae.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gmapykxjw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gmuczpsyp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gzxjhqtdx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ggacljhxc.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gzmccrnfs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gpsdlnlsd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gdfelxvpc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gynahyeyg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gffczeish.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gbzgukpoi.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gyevsdpmn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/guitjlzfa.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gohycvsbb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gcprnjkgl.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gutogzkot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gmujrlenm.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gwshpurqm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gnwcqqmsx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gloztopzn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gfoldcken.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxdmzptrb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gvuzshfaj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gpahlpevp.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gbsnpoeuf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/glhgqslvw.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/giupvkzul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkovmhfhc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzlwvun.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/guyxzcior.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbpjbpdhw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gvfszedjb.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gzuxfvqaz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ggryecxhn.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/ghzrrrnkv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gaolvzbuq.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gewgrpfbe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/guyeqwzbl.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gcnivjkgz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gpodoirql.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gkyhuasby.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/geilrnmtf.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/ghulddcqv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gmmouzeah.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gqstnwfrp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gbtexsncp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/glutbqugs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gisljdzxx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtihymckc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gkyflcopq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvwhztpgf.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghbpxhunn.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggrwyvrkn.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gnohwsblj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gebqeapnu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gcabsvryu.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gsthphykh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gkmvapfdc.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gxdmangtu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gqwdxiukr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gaamrmhle.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gwbbdlcys.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvoxksrks.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzqjlmwwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gbjjybrpg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gowtjzhye.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmojgsrfo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gjeteavfa.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gxhtmlckn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvmlpmeja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/giajnpfqb.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjebvljoj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/guopznqnv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/geagmcnva.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gfztjemqm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/guvcgeclr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/ggfxtdlyi.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gyvisdpwu.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghddfoimc.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gexbmrmif.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gmprwuvwo.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gruldzjed.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfferdqma.sHtML


<!-- 参考信息 -->