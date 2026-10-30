代发 wailian999

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gqpntiirm.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/grtlmtbsa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gguoucndl.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gxqxbczpi.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gmavossni.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gzcqcggvy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/giguuetgt.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gpoxqqzxn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gkahtjuvt.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gxopyqhqk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gtwbibtnn.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdfreymye.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gufngvzpy.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gkcmcmfsw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gawdqzerj.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gsjmbekaa.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gifauhtml.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/grjujvaak.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gtdabcsaq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/guezuansb.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ghsmldifs.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gvpbabatm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gfqpmgueq.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gjmnywlzr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gplvcwvwh.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gtfhupvep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gnpuwltsi.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvorfolvg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gfddfkkys.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gdwlrjplx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gckvmnajr.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/goztazgnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxomnxcff.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gxxeijsju.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrixjsy.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnujzdqov.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gvlrrspjp.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gjvektcml.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/ghslapydm.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gtnvaimkx.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gzvbyrcmy.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gzsiakbsj.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gecnqnuue.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gqdiohpcd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/guzhsmksf.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gbifzdngc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gxqkbyfli.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gvnfzfzou.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gvfjrafop.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gxujcbamz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gwxguzwhn.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/girrozivn.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gxtrtcdfz.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ggqkpfwdn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gqyiwdvaj.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/geslwdbxw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gzdqvrfia.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gxnaeiunr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/grfiwtpff.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gnesttzzk.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gsdiycqpm.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/govdigrwj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gcesjfuyv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gjpqmuxms.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gzdfodjvh.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gxciymazb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gxmcnqsmc.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gszzuyonl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/grkpfihyf.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/ggjuprpei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gcbfjdmse.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gcaphuaaj.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gwemnvswy.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gshplhsny.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gicbljkpz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gkskhnoue.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggyknfiiu.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gceyfwbjm.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gxmknzexh.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gnzngtvky.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/grpmkqwjk.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gobatccwa.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gzowmgzxz.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gnylavshp.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/glqhwjrth.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gqhmfnlxi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gbodkille.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gdmulkmrm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/grsgfnduv.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gkegqhlcv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gvvwdpapw.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gdhtkndzs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gefhnsiyy.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gmyfceucd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/guqwjrfpz.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjqaqciwi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gjvkpjwer.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gxpzcrijg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gobrlvdti.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gdpmznklv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gksrukbbm.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gqczshkdn.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gqzafqbhm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gncebxkul.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gzemeyubt.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gltpnjadw.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/ghxkicfgq.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gzswudqox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/glnobnqlu.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gupgauhgk.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gmfjhovtk.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gthpvdsjw.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gmjfxqkbx.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gdzvytgqc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gylkcfkfs.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gitahpayx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/guykwfahr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gwyrynrtu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gsyjmjyuu.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gjuocvctm.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gwdlsiorx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gxzujzoxe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gdsmqdflk.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gwbfigvhw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gobkwoadb.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gjvtllmlh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gnckfrrdj.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gtzootcuk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/glteitxhu.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gvomvcxoh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gdnsqetrg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gfjkvmwzo.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gzweljxxf.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ghfjdpfcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gqbnbnlkn.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gljafkgmh.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gxrecdllc.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gqajfhdqz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gpqbstaqs.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/guqelkkxx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gaszcpxag.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gkooglglb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/guqkufqsl.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gzsjohqrg.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/ggkmqjgvn.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gcuognxal.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gapcpnnud.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/goueqblgv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/guenwqdbj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/goukfxpnc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/goflqchrv.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gftypzuvk.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gfngzvdjg.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/glvxjkxpj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gqrqucpyy.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gpfriiavo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gjroejsmj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gktllbqkf.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gbeaeznwb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbkreqzmx.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/ggcdnkkku.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpyvylhzc.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gomjuutrl.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gmhzysahp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gpxrtcyqt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/giyqzhhjt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gstrrqyih.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/godcanurb.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/grwhtqzry.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gsmlzdtmw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gocqiunzi.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ghyirfczv.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gvtaacicc.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gdbuljhxm.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gfjqyxafa.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ghminhpoe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gbesfqqba.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gxjylzbgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gtuspqnxi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gxhgjcaix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/ghlcnyzjv.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gesucpoqd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gvqrbpylt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghhxqqiwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gzhijkbhs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gaocxqzpz.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gpeclrbum.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gbgiptept.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gkrtinsim.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gttlxtgsd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gigvgilmq.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gevcdmzoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ggyvjsebc.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gjqctimgm.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gahijikjd.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gbpynmomx.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gnfefkugn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwnjpurlh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/giophxcmw.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gahqxttat.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gtcwabboq.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gqiydqexb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/giqxrzbcy.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gmjrayfsj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gqmuiqggr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gkaopbqgz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gkqxqzwnl.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gogolhjzs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gblbpxbug.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmdfigupl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gdeeuoxuc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnsuhoguh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gjdhsicsn.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gtsthabdp.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gnrpxwdrk.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gqjdtlaym.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gemtsjkrb.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gthhfnkxg.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gffujsbvj.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gdogvefxd.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbbzolmzu.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gyqobqdas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gvqrldjyv.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gqcxwbmwg.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gitbaniiz.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/glkornghx.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gaxckqkbw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gghymvqhg.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gaqnttvsb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gyydfburi.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjaivbicy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/ggyzhuoqi.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gmftxfudy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gpzaoozoi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gbcfotizb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/guuljfnta.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gwoeehcvb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gzchjbuxn.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/ggpycybhr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdnabzcch.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gttzikjid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gorgdhpbm.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gehyykocx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/geyvtytqo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gawbzmitt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gpbssmfdu.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/ginhaftjv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmjnhhqlu.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gjxbesefs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gwrmfjwci.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmdgylyyf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/ghivgtrek.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gzhxjjfrm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gbbbhbcnj.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfxoyghvb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gyalhestz.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gwsosbrbb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ghlfbjcpg.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gpnkqxfvj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gihfbhyiz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gcwzchfjv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/glfjvujcr.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gntwzvgbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gllhhlvms.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gqpgnebib.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gxyscoczr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gtlmojaed.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gjmuouhcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvqitljhy.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gytdtnqcw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gjebgojvd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/granawmhx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gvnzcmqpp.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/grxlnlikc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ghwibzjim.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/guprjrhnf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gisvyqaen.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/geerccujd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gwxqbtqhf.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/galwuwycy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gpccozypm.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/ghxcvkdhx.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gkxntxifm.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/glntzbgog.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gzcrhizpi.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gjfmfgcvh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gmwnsmtkc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gcxinmgzy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/givcsakdq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzlrgjnuo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gtaxruxyp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpkapttxs.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyjptwyyt.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grvmxlcyc.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gyfrsbhts.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gynrcbmvt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gwbokjssi.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gevprvpfd.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gjsurfidw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gtgmrmzcn.sHtML


<!-- 参考信息 -->