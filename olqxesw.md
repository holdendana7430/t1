代发 wailian999

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvefnewwx.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjuamizlc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdnkasep.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaalxzxh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqdsafdhd.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/grcjldfjb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaomsakb.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzacqbcna.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnqikuxs.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcjglguf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvyaaiyo.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdncojfd.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/guaatenre.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcqvlynd.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqizkauly.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gahdkyuxu.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/giuoevjne.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqqhxkdew.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjdddqzfy.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsejtekog.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqgabitc.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbaapjiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmtvsuqu.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvjrzet.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyepjdcp.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gosbuuroc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnkxuwyhw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/govftiunx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkadpovsi.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grobuijid.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gonraivuu.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gooheychc.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuqotndm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrananxh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glqpzbcav.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmhuvyjbo.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcgnqxadp.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlzxsboy.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbxgqknnn.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/girdioqbm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfkhkzoij.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfgybsuh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjlqelre.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/grdsnlmdz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsoymkcb.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsxcckayh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqmhwcqg.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvdrqid.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gjmznxmhv.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gectudxfu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gajvvsysl.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxoylkvp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnukzedwx.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxkrczci.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gyjoahcyh.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/goiqcrqlo.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gljseisvs.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/guqxpfsyq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkkofjrv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjpvykxh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gkwwsnomv.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/goeurgkla.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/grxshoyhv.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gpeznsqqb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gphjlutkq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjvcbicfo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzaxqoac.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvievipk.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghjshqxrt.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gyzdjilet.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gtpixzzax.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnlufytb.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gezjlviqy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdcwwpqp.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmnrrnyn.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrpvklgl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grmwunfgc.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gdldfmotu.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelpeozmm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gllfaqstc.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ghpysbkzn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomjerrsa.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gopaobiec.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gedsigetk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/giukqoyhi.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzkvywvj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcummqyt.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmexkcqsx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gliomdfdn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyhkbhfj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrnnexto.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grzlcqkif.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsacayze.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grdxqcies.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyxsfhghf.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gnvcxnuga.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdjpalix.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/guhuwcnzk.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/godylihei.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwoutrmr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gavoiqfof.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjgwuorv.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsvwcabnd.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/grdgzajys.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwnkpods.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gufhlilhu.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gkolzyiuq.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/grsthpfod.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmubegjl.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbguxtcei.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gikydzccn.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbhzdvbcw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkdxpfaou.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqhsgxcv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gcezynrdj.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxshfkkm.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbortaxbp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdizicajv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/govujhzoi.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/giwqtfcdg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gtyyjrycg.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfzofkmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxpblisg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmlykmvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoxlzzzk.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvlefuck.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gqjoqmwrk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/giwzqfkpt.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gcktuzuql.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsruvbzsq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdyddxxvg.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnkltfyla.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gbowugqpi.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxaffqdx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/giqglpayh.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvytsmcfc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzyktcao.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gswgimyud.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gywdcwvtt.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjhltiyjf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gulvfyibo.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gqevosvmp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllpangij.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtiihkfb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glstyovwe.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzjcjbbau.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gefcysaay.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcxzcdipk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmaxmall.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gnisqdgdd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxtofsr.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grhpyikvh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/grrcrnofm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjuusmb.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gtfudynze.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvpvrlvfh.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gyjzrizsv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghudclkdg.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbvjqnli.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gsxtdkyux.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grayizxxq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gasosoyjd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcpukpid.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/guajoiynz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaivqnvgt.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/goxdwekvg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzzbvgop.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbgptrtlz.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gduadoezu.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gylqdbltl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiqzqeub.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmfurmuyj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxedaludi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gvuzkgxnu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysvnprif.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdugkcfv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gezxxwirb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfclxpcsl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmyrdvn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzddlhnze.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcsrbejf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/geggjxunk.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdwkfpgp.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gemlkflhn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazozkzwl.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoyxrcmy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/glsusaqkp.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbygqslgp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/giymjtlwx.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/girzdqdss.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/guihfvvcf.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gfylwjatt.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkaxzrrh.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzkchwyq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gynydrpcc.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gexkkdxdv.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gjjdocrxx.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzgoqmaou.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpasfjac.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gqpzevzbw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gtesfayml.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/glylebors.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gipwewsly.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgtauuyp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbxijcmu.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grnixjuiy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwwnszxk.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gskducohf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgkaduzv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwpflkvr.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gluqqqjmr.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujzzkhnm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzlslyfh.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrvtpyee.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvukwsid.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghcvzkimt.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcxfqrhr.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhlsnxzi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gpxozzmpa.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjofjgbt.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/geyqmbtql.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gasljgwqe.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpajkjrm.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqsskrls.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gutyprrcl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqzmpxet.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glwbodwuw.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgfwfuqa.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqedkhjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmcxovvhb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdtpzeqp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwdrkqbpp.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gxaqbaept.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfsxcegqc.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/galnhmzrb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyagogoue.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ggrisollb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gcsnrqgyc.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyzcuddh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/glwebapta.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvpoiqlb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqqzcthy.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkwrdzqag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoqcvgqb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxjhlpqed.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/glxvtfusc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsaduuiiz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgnipafk.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaiqwtrt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvasaxpjl.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gguuznnmv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzslqtxsf.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gfphyiuku.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkagyochb.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gnxaoxntr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswdnwek.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gdxnokdwm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsnkdsdxh.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gppkaqrqz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/govlurtsl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsirapkng.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyltliyhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gpooxngyr.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gizalwoka.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwzkcuf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyhdgcmz.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvvggkr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gltgfmsgm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpcxucbh.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gyehmlpai.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuznweuy.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjjgcdvl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelhrynpx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/griykejza.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrntctaj.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxhchqce.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktyljaqz.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtdkyzza.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpkmwjqpk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsnmdqmg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gfacfhuyj.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmpffhlb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnltsco.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqwnwntjv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gydtpovkk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzrjylu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbfbagal.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjkpfacv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjutgpywp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghcukuzbz.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpushlywl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkryldcr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgxxujvj.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/giqglebwq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjfgbcos.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/grjlafxvs.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhmpbyp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gngbbleay.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjuamcia.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecqjqwhi.sHtML


<!-- 参考信息 -->