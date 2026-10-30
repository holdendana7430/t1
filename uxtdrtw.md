代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcqomdhp.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbenqzrrt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdrteyky.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gbrifgkpq.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedralkad.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqerykfr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggclgibfd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzpsiskh.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpqqpwhf.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkauramxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gavcclqdu.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlcttccj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkoxnoiq.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcuiesoh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdukwyca.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxfgmtml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdbyamwgn.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgozakmr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeqgbqcr.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gbaresdpi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnxynjthi.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gzivcaomk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gobzpllow.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzbinslce.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewkjqotn.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gwlcxxscx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjkbozue.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdlassfg.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcynaxgyw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gzlegmcgu.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpahaexpw.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gndwymksf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjtiyjvt.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmkmchth.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/goztoderg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gqwovnbss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsptwvhqt.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzphqemhg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gvqmfvmsm.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjevtthy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gawjpwpsf.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayqtaqzf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gysfzcrov.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqsjqqgs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/geujtczas.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkpadvmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ggcmbirqj.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmglefph.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmwwauss.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gskcxvkhz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gclhxgwjz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwmdpoez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmmyciza.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgbycwag.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guywhgeqa.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvyaginu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnmduimy.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvckfmttv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzpfqhwq.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gowftquxv.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnknelneu.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhdsnkyv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtzmqku.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/ghfunlkjk.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtzowafch.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcjkfjqs.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gxjaksurd.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuqsdora.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/grypvvsxo.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmnkcynt.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmwocyhr.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ganvfveoi.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsvgktgc.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gfovxxuns.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gstznddws.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gtifnokrs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpaqzxlg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjkiakfa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzscjge.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbqezakh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzpylvob.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbkyrgzo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gluufanng.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gluojxtau.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grdtkysvu.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwdluiqmi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guktxswrj.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/grpinufax.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gaksckqhs.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/goskcmrta.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsksanckc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyroddjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gbuhrmrzs.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghchrgnny.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsyntjple.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/geehdnovf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbkiuopx.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvxsmlsx.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gcruyfkag.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gmlgnrsul.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvrpbppd.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkwhpqpu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyjmswrq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozpifwcp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjnlxhc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gpjmxixyb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqsvfuqhh.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gfdsyvdxg.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/grzpjkppt.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggqvxioll.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gwhmncrby.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfqiusfs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwpdligu.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gigtohmvh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcujjcikf.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gndcohddt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnixewef.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjwahzdv.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gwdxzxcwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grddywmtf.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gplyqnxhg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqyogwil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guldqrdku.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gklbhzybd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlglizfe.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gxoytmjnx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gdghbmfnw.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gefvxrvtu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyczfuevm.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxhgjhwu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gaxjakxhw.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxdjlucz.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gcvhfrxbn.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gyexaueog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gegylpyqz.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/guggszvjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweuoimlb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlwdcqno.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlwibqoa.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbregxcwe.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnzhihbu.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnmpjnel.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrhrgblf.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjknura.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gltmzkzad.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtgmwdbu.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/giqybuwpl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzscgqdbs.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/giqckeeed.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guwcidkxr.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytcdqfwz.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gklyhyufz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifvrijrk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/grsgpjcjj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqltubttl.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqigfudc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvvshrtd.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxsvfkswk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkyoesgq.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gulyapsns.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/geprahlao.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gaxnaockn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgkfwoq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfqalvsz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/getmvxfbe.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbaxdczw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeuakjkl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbatrwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvxujth.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/giggarvee.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gwchszyce.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxgojmc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbwfonte.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gumxjokli.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdmmejqsb.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzoshsibb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfwicrg.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gsezorfda.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdsqrjqk.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghfhgofql.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gziqkjvyb.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzgpomdvc.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gejgfcqps.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdgtewtz.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gazpncfxf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxezuvzm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbkobnjl.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjzodjvtu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkkvaiuf.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/griljpuev.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/goyrbndnf.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggxzlrxvf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrvzosqx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeyxzwwh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwhfgrbd.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqnywtwrt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gzbtqmqeq.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrgwanuw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/geurhxvsg.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqgtdewcv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/glfajavnh.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/guigvcjlx.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gpsjfynnp.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvwqujiq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxdsxjro.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsosnpkwy.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycvicbvx.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcopuwyrs.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpisvqva.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjilrvtgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydewbdfu.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gxtryrsni.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqsgwswk.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/grrdehkfi.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gznpdxdwg.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxtjhvsy.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/glouddmad.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gunnubwwb.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gygamptnr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjwitrse.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ggamlxhty.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdrldmf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gbntwjktq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltvlcydi.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatlgyxcd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjgzqxdmi.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbxipvi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gocyssrrt.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gqgyvuolk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guzkztvll.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjslluvff.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprhkrrot.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidgwmexz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/ghpusaxgz.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxzyqlplk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gclcdcfzk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvaibhlee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwlbslzl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvvsziocz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxysalc.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gcambpayx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gekqdzxbr.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gurxnswgg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvtonyf.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gxshpoezy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gyvpxxlmv.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghshkncon.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghafotvlp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gyijbmmyc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwsmnudkd.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/guqvklojs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/giimzbzhn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/guufrcvsi.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqzdhjbh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhmfjcyh.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggcekdjsc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gemvmyflp.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqbpfhca.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshndxxn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/geoyxiqqu.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbjtdyla.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gjczapzbq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzfziexd.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbrsevy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojxoqdwy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwxqpuya.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjklazpm.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/glqxsiffc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxiefpxxc.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gflfnbhsz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gwmhhwlce.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/glsiybint.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaytinhge.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwiplbpx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoeorpul.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsurchqc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmucibw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyzpwkyy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvimnrs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gontfzsdj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnrjjpoi.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/getfjfpos.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvfxsmsp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiytrwib.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gadwxzpqy.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gxzyzrpcq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gblejuacc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdynzsdk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ghrbtbgla.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gbvdnrisf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gljseaukd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grvixuaxg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqiewbs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glhzsdarj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjiadcrj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbjqvgoo.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gompdhnzk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/grdfhlvhu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmewrxsf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gyagovzir.sHtML


<!-- 参考信息 -->