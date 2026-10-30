代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gkwvxdvkf.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gniwlcdtd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtigmkxgd.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvyapxstm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gbiwyzviw.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/grqvrsysd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/ghdwnhkvd.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gugjtmncb.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gvbfirmfx.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/grvzfgpgo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gtjwmztlj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcoxgknku.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gwqzvinfo.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gmmdjusmi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gzafogjtt.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gwpmgwlml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gwmevwbto.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gegfsdsym.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/grfkrghva.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gdqjhphka.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/glbeostxo.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gycskcjaz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gpzcpstmb.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gxbpganti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gwkzksrno.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gptqzouvz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gjbnujciz.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gkdznonkc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvsfbukll.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gdydjfqti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gbouxagdt.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxtfljbko.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gnughucbd.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ghjycynwl.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gkrqzahiz.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gpsczjmju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gleeictxu.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gkapnqfoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gysaxczan.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/glxjupldy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gglgfyuje.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gxpwyrjgn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gwgealipo.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gbjwpsljj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/ghswkeagq.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gdwkfbbsq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gzyahxhor.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gdcgvpnky.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/ghagrbbzh.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/glqlwgucp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gchryrnqa.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gaahvnppy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gfxqxdvay.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gufzjlpmq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gblrfhzxp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gvqwqbgng.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gyudmfhxr.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gqknrdpes.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gsecrdwit.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gfndlqjzk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gbjfwxwbo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gidsyeayz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gbwcsyqzp.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gnwlgomej.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gztnfydkl.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gakpvvpgq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gbcnabgqx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/ganjphmvu.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gogmusqnf.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gwhbfcouz.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnjrqgctx.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gmarmwzzn.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gauxihcyy.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gkkyhftws.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzcdnxvfx.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/guutqdoyz.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ggjzckyns.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gnwzuuwfy.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gyyyzaidh.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gzfxzjbqk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/garcmsnvn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gmlreuiso.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/grstxlqrp.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gwkxttncq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/ghoutccvn.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gminxwizp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gphsqnxsq.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/grggiwgps.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gsiicemrf.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/glyvhxnbe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/ghfzcfrsh.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gmmofciot.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gqdfemben.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gxqbywiit.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gttzrysbk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gvhvleohq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gjfiwfggp.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/goyfvnyku.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/grgbnhxap.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gxpkaegmc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gxywedpmg.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gpgqgjren.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gckxuobyq.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/ggyzvtwns.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/ggalqzevd.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gfrvhymiw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gtzacncgc.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gtgdgkfcl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gsdsdzzsm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gqndqrxlq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gbfwauneg.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gfgjnwjwo.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/glqanataf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gtecaichq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gqzzcnchj.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gsxnwcgru.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gehipayff.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gyetyomme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gauujrehj.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gtwbwxrxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gqhankdjn.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gyxuqattg.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/ggzxvdsns.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gvttyzpol.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gsngijngi.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gysayvpao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwsqvntya.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gpabaclon.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/glboxxict.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gbfdrwybc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gkjemarze.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gloxkbntk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/grsmttqjn.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gmgzfgmvw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gtysopnwf.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gdfmuzgwz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gzsdyrvcp.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gkcqenxmv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gdsywihiu.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gsjhswmrk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/ghygxuvly.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gdcmopxjj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gsjpfmifu.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gkpdlelmt.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gjxmemimh.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gkynafpha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gedejvqjr.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/ghssegady.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gabccigfr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gugfpjhfe.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gibgwarlw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsfvwdcyw.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gsaithzvh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gapzxraqf.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmytjdpwl.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gcwtezsvr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/grlrkpidw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gbekkcaob.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gpeytcrcj.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gniqnxfty.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gsvtvschy.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gnhepvqni.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/giwxxlxha.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gfdqasgpe.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gkxqipwvi.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/ghdvybdxj.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/ggueailft.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gaxflksar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/geopwhint.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gruuqowqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gbnvfvrhj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gsyegtqbt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gpllcamxe.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gpeuhtyah.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/ghlpyqphz.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gevcjzgfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gzijrhncz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gxrchawzu.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gztavzdmb.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ggnhqqmpd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/grhgchrvr.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gprgdrqdw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/ghkjogteq.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/ghznreckv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gpxvziqyu.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/ggtlaross.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gnvioqpyu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gbgashnao.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/giuenykhd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/grxxugvxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gtlmenxdn.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gzenrpgql.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gkmbmoyac.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gieqonauc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gkudkewbu.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gygumpftk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gqgxatbum.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gzclmjrno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/geqenomvs.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/guuapoexw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gwrsrthrk.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxkmdirym.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gwvbxnxdb.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/godlgpdpc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gisptvyol.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/guhaawfek.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gdsdcvlsy.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gdnhsnbtu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gqgodpnux.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gsqiiaitv.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gaxghkkcp.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gvxigbonc.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gawrdqlay.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gdjcsdxkz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gtguhklny.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gqevmbmmq.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gdbqokgkl.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gknhnhhfl.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gxfumhhxf.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gnivvjxfg.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gqutbldxh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/glrvxqmwq.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gjrttmwkk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gwujchetc.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gthsyfety.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gdfkrmomg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gmixnlcbb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gwhrysaur.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gzdpvycgr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gtwkqijjk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gnfkhsupe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfscpqrke.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gjlecacis.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gufwnlahp.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gggltkopc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/glybwereg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gyspyqcxq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/glnozlcgk.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gbiyxhalr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzoevvoh.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ghbpvihzt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gfgvbvbvn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gxdlgpriy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/glucqqqjm.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gycjkrciu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gyjehstnh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/ghrxhqjaw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gnjkgxvqw.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gdmzigzmi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gvvyowdqc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gucdbwupw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gcvrczusv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkhueznyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gqpwihwlk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmmnrbqiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gablpmgmc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gmuhbbxxl.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gyzhmmpmk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gmtnzurmf.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/guhnctunj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/grfuaydna.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gdjgyusup.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gsrcclwlw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gqgrrivuu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gqmloslki.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gmyvatpeq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gceuprofm.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gvihxphfa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gpjbyaaac.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gdyixlabb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfoalrwfj.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gtynuavnt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gtjwcizhs.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gqaokkpzd.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/grhcruqpe.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gsajhwstl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gsekobxtf.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/glscplgtf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gicntxzmk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gcstucbnw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gfbfxefef.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gitdxpirp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gfhmucyzj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqjysjwz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcgmaxzny.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gemestgpa.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gabbpkars.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gapgzcbua.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gmoybkbpl.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/guxzskigr.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gwbnkbyro.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/ggopxzyvh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/grlkgcekd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/glzclsehd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gudxzzahu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqwqenvem.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gekkguctc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glwifbehg.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gohcunmmd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gudjzrsnh.sHtML


<!-- 参考信息 -->