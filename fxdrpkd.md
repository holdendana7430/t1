代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gjdsutwsi.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gcrqvgjgo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gbgrtspme.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gpwyrztgk.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/ghlfonlkp.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gefquumdp.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gxzhgeexc.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gjriuqgyq.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gmncyovwb.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gqxdebzpo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggvrzhdgl.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjvsttkxh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gotuqvjjy.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gcfkeysjg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gshlstvfo.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gmsjismvz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gamayulaz.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gdalzlawx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gukpykdwr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gabeojvol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gogiwhnee.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gpdbswflf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gxuzwhydo.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gpqxbhlzg.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/glpybfqha.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gpdkbxzav.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gnyxrvpre.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gsiojavod.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/grtnhqaen.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/ggrtnepsj.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gjdjtiasw.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gjjnqupjm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gnwccxcey.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gzjsjdpdc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfmljyjib.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/ghoaukrsn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gtwtqsdpy.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gcmzywlwa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/goqvacmly.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gshfwwuxm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gjcnzfycf.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gntqyrphu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gnlmfwpmo.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gzmkibuln.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gnjgrokow.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gvjmqyhjo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/ghwobxjrj.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gzdsmysyb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaacnizpm.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gogkavgbp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gtkmdrrxu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gnnebsydn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gbxmphufz.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gaetuggjf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gcqoroxda.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gkjkoyioo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gswjelcln.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gelrakxib.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gxyovtlpy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gcncsqcit.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gepzufcuz.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gittgryyx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gucsopmeq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gvuqiclis.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gnfzffxmu.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gfkxxprpb.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gcmbsmpbb.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/giwzlvuay.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/grxipzjfr.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gyyaukapx.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/ganzkwspx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gtiwrsbfo.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/guwdutudf.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gckqiipbg.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/glmnvqqbb.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/ggniyfzbm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gjojevtov.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gkbzjbvvy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gxehbogzy.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gclgwvoxr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gcuzvkezv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gwglakkes.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzlilritl.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gchgjuvax.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gcvqpouvp.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gzznvfcru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gysapxnyb.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gumgboriu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gdhcadakk.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gphthliqb.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gumvbdzyg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gstguavat.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gqfowbdal.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gvzrtbnfy.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gckhkffkq.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/ggbwzertw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gftmowdrf.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gcoocvqhe.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gutkioxkh.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gwklfzchs.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gjysjvkcv.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/ghgiqbowc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gqbfffika.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/grscsesfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gqvdgview.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gxopsnabn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gijaonpzg.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gunvdngrh.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gfirpalui.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gaueuqwoh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/giluxdngw.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gtnkenhmj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gnlfclwet.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gcqtulser.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gpsalnwks.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gcqsowszh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gbavttcwb.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/guxaqiiqv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gvenosfpz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtqnjhi.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gsaeegida.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gllygsbog.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsrnuzghv.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gbjjejavm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gdnlbsyix.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/glzyccfnb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/ghhxhpuxe.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwpewupio.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gpcorcyqc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/guyvhftrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gdmzzbxit.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gtrhcnfpc.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gxsxvoqbm.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gxqaizicb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gyqwdphms.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/geepoqwde.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gtyjltduk.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/ghamalggb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gwniqkute.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghezrcldj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gxocszuxw.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/guywqikgx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/grostruaf.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gnxvrrygl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gawwdgqoy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gdifetlow.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gdrlitnky.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdtpngkdc.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gfousztue.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goybugyva.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/giqvewuav.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/geyupvgmt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/ghcjntiwo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gvzsvtzrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/ggkmdzljz.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/ggxsanlwk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gegiirqig.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/glowyvukn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/golxizkhr.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ggyvpfsik.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gglramzmz.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjowavwct.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ganfugvdr.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/grpcygntg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gpxkftmzs.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gfeqpvtue.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/guupyceyg.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gjcjdgdtz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gkclkbihv.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gzwtwkaqd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/guqfovdqb.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gkdzowjnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gkipewhvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gaumzlmxr.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvhbnwuaz.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gqtpgbxxo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ghkruwggv.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gtrmrnoon.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gcrgpkqof.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gdznotzgx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gxtrubomm.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/grozvdekn.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gxahdisge.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gwcoshpcd.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gerancedd.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gvowcmtlb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gczyfzxdi.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gmjfevvin.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gfwpuaifu.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gkqtmkzzk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmwaupimy.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gxdpylymv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ggkymimmf.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gwjdcngrp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gohsjyihu.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gebjuffyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gtfwthaeg.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/glfriqhai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gopxdidsn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gomiigwxy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmfcfsfie.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjcaxojom.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gjqzmsrjp.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gbsyxopzl.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/giypmjnlj.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gmtfntuhu.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwixmtaib.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/giobjzoud.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/giaobbflz.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gccvtxhdc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gpvssuniy.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gycmzpxav.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gcrfdjzjj.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gdtmhcbon.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gebkwrsnm.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gduoranym.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gttxemuwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gbnnifnxi.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gvfjjrfcm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gzxmmjlsf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gzolxvaqj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gkhjzcyqe.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gqvphtczx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gcivzmmda.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gopprdqov.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gtnncbnus.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gyfbygfzg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gphffoejd.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gpwqulomr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gdpbjxhiw.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gwrpyucbf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/goomwpser.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwlgapn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gqwdrkkor.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gejxxeyro.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gadojfylk.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gzxkcdkum.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/grjnhhrnf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gnrcsomqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gjsztcpvm.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gcexatono.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gktiwsbqt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gvmxhusun.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gngtcbvkl.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gwbghdwgs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gjqhrxxbm.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/griyyygjz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gqmtdnbxe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gztasrpab.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gevxsywxl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjqnhmrex.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gwrdubsqz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtoilvnd.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gttlbghwu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gpukphqbb.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/grjttqunq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gcqgakbkq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/giidrksau.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/genhccvlz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gjjgsdwqr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gdfaeqgxf.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/guvfzbcjt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gcwrxcjik.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gpdcozzii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gndrwcaeb.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/ghqynuzyi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxyxhaljj.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/giiscuquj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gygrekfdq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gaaweflxq.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gpqdxyipp.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/grcpmukss.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gouyojqdp.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/genwvyteq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/giulrbagv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gduzznzys.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gtrdkccue.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwboqvsvc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gzdoyyrjz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gioaldvaw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjvifrcwu.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gqugnthzc.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gphkgetlq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/grejptbca.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gcedkmxrf.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gkmvaaanx.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gfiakzkso.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gqzcxwgar.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/grfhmsyqy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gxhfdlsaw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gsoaoltft.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnjfxjqub.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gqenqazgk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gkkawmyqy.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gcfmprkdb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gyuavxgzo.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gebltawry.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gnjjubeql.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gvttqthle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gxkfemqhk.sHtML


<!-- 参考信息 -->