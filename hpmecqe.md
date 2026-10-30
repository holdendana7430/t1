代发 wailian999

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ggfbckzmw.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gexgdhegh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgexmyqr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeiaxihz.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gkyrkfwic.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnikosswe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfputnsue.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/goqttivbl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/goutiuang.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gbvzilzkt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzuseaqd.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdpeqgpvo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmsrvzqd.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/guigtbscj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvweclan.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcrwlqvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxxwbix.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgiweltn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmqzclhq.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gztwemgsm.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghbwnamvq.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/grzzosmbc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvepyevos.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoafpcgw.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcieyimcw.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gysbnfuck.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giflcledl.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvpxebwmr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzluvzqk.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gylzebisj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchkyqeaa.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gtitpsyic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gowozhynh.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gamnlsbvk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gmhvxzqtr.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gucixrqma.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gasralzvd.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gybmwhkjl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/glzlskoeq.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfquvhpeb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/grnaiulfe.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzixtifgz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoitafju.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqwtuelz.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyndzrrjk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrkrxvod.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdnwthvfi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlxpbmnd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdmvqiiz.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gtxzkucaj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkshdnqia.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkiedoypx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhfemxhy.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghejldphi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/ghzqvkfwe.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczwkpchq.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclgqkthf.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghzdbhrqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkutxyig.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/goxhhtbys.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/glyifhfks.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gitevobob.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gttfkpmzq.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gvdcyzmat.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpyftwzl.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gojzpelkb.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gurubsgmm.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtipytyc.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/goveggsgv.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmgojqfil.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gjdswgbod.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginnukpmo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkffrgte.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gifbkbhgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzvsywyi.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbhmuois.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gapkcpegz.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnguwmpr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcdhroew.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grvjhysnz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/getneecag.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywwtmvst.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuybavgo.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmqplvcxo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gaudktrnk.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gwidhxajg.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gebrsqgeh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gvbaxivli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gajkigmzm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsafngnnv.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbharptxu.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddqzllz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gtfrvydew.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvzfddx.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gykubsmhm.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gusagsqdg.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gmradybtw.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnodfssex.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gvxtaaovw.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwkyzlgns.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gsynqwpba.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gflwkwskf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitccouvp.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gajyfbyrj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfpvcfiv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkqnktyv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrifyame.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gxrhdyxnn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gtayxzhrb.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixrnrydx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxpirgc.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gwxypqzoe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/guflybaec.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtxlgefbo.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gbqhpygot.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/goyhgjvlz.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gacnyoftd.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gaergxmwg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfubknmul.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmloorjhb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gmafqmuqm.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsbzbyku.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/grscehiux.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgmnydfx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvevwiis.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/giikpnlct.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxnospb.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gowyhitec.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrpvifsi.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcenlkud.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gypzmdpfs.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gebtopego.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/guihpifta.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gggpypchh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/geuekpupv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galpufwsr.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gihskkkmf.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcrkocx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzbmwfqg.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgxpbaej.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaliebww.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gqvyviizi.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gmjxreyhc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnwtgxczj.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqywiozl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcztjvitl.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpwehgv.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gftmfwapj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdouayfnz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgpgxbdn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzftzhv.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmgdamny.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gmtewfrzb.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/giuznumgr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gwppvpkao.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gundulmnc.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpgvwtbqx.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggloobnhc.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gozskgpju.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gnkisfnic.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoifwoxr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/guspmmuyj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjjiyghh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gldvgccxj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gzacabdte.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gliiifvwy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnndyvefn.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjiqxluc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxpikam.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsadmvbc.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwexwevq.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrjtymb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/grkbkmcpc.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqdamydi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiwmrhpa.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkgtmgz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatqyiehy.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gaeysbzwr.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/guttpwpuv.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gnckjuxwj.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoptzukv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghrhefyem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/galnsxvjh.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfzruzyv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazdeqckm.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtdkgjeb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzrgyexoh.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnfwjodoj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gbzdyoizr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gftftedvp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gneriwuhv.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gaatrvgnu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozllhbib.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfezvowwv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaiuzhmb.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghueruefv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdppkilee.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/guzdnykfl.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gchxhyjzu.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwubexh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmdgrody.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjldiktrr.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjreyoat.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzixpvex.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/giturirwi.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdaxpiqfb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbyuvixk.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gtaqodxzr.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gffhorzib.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/govrrlzen.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzvzxvxgf.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggkfglvec.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gswhnkhuh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrdwnryp.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwakbgunt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gxaxvrvae.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gbevrkzhb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gpmsecpwo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvdguji.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbfgijlyl.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjmqygvke.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gysfysusp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gayjprzvz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwglycuey.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gugsxkkvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxppkkwrr.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszpowlsx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaaofbba.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtgzeolx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnchhrmqp.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gogjtcwxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtwnombk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbzisttw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbpagnvih.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcrcjsuuc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gznmvwywa.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gdymqwpsp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/greggugfk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltpekomh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgglqihq.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazckhlea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtprlbtia.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxhtztnl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzpoedibs.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbinyuli.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gavbwlltw.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmutkkxap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjyyqrge.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwkpgmva.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geuirnztf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhjqvpfx.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gdmofdiet.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gvoouhrci.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkidvyntp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsicoaljl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gxactxpnn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvdymqlm.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gulffkdgo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnmjlmiz.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gabjinrpg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gutoyjcil.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gduyekiep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomcjfrke.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gvhspcgms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaboaznhs.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnkpabrp.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/glsgmmcwo.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/guaflvnts.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuvbkvjt.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gcxseihue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyghnlzk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/glodfveha.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlqigpcr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggysbladx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/grxztwisa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsejgglcy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsvrwaudj.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgwtvama.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gglmcozfs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gvjyvqdpt.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gfalzdaic.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwibowsgd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gttabqemj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgkddwep.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/glypdbixx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoqrcect.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfvzatqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gycskggoy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagirsvtf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqckfyez.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvmtdvdp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gcjmumpem.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdwnqpfg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gdyycoifk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggazynnwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/geqrqizxp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwquticg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gfmlitbtq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxbxxmqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdnhnfsdy.sHtML


<!-- 参考信息 -->