代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gwkcdrlnu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/griixjyio.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxfcjeqkp.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gnhmlmzjx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gcijgusig.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gpndeadqe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/glctixcgo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsxylrauo.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gonztcegz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyoqakavd.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/ghenydjua.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gkzrzzmdm.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gpwbsrozq.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gnjqnhdwj.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gmtsmqhzy.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/ggnunfsoa.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gcdagjxes.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gyigiotoh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/giymwztzp.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gdyaoiace.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gknyrcxmw.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gjtggwxwd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gaxqvutzc.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/ggsbiddam.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmgajmkwp.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gjvzzsqqu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/goyobdlel.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gptmvydep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gzbhsxkcj.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gnhumszze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdprmbwum.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/ghuulmken.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gnlrgxlkj.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gicpleibi.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/guzxgzdhz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/geyggqamr.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gxxonewki.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gsbybskrv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gnnuzyiit.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/ggmykyhzi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/ggvylniyh.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gdenzfwok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/guffcljyc.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gpipkqcjs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/geilqkxqk.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gisrxoobh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gytqdbogj.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gtpiugeyz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/grljcgjrs.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gvjnpkxpx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gnkjgjkym.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmnpyhdtt.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gpdoxxhkf.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gqklypown.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gawvpahbq.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gbzvhgyod.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gdlzpvokf.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gjvnlqyyh.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gamygblrg.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gewzskunn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gsjxdusyd.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxqgduily.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gakyfexns.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gacyipxay.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gzawyzudt.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gaqdzgxbs.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gqqagjyvp.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gcwbygkyl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gkkzpxeru.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gpshxnixm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gulnrlaeg.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gscaspqcb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gayczleft.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gtyvvlhou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gztnzldtg.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gmtujucmz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gqepyaoeo.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/ginoudcfq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/glanalphl.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/grfpejvqg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gjvfvbofj.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gqpclztho.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/grrrqxgcg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gcacwmtwg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/glaxxjxgj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gixbsoclu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gkmqjifxe.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gokhsozbk.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gwllknxma.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gxesbkmow.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gttnehzol.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gbaqsskwz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gddgvpanl.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gpcpftvnl.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/ghcysshqh.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gyciqrcqp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gqdmgebok.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gyprvhpcx.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gnekburru.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gedypbmuk.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gmepvnoyg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gkdsyjabz.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ggtcicymu.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gwvsxzszg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/ghoqmgcin.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gzjiilakl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gfrtldzzp.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gsejfascf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gtoginhqd.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gnhgyvsor.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giexupicv.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/ghndjtwiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/girpkuhzt.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gjpruutqa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqwdtspgn.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gbelvurve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/ghfyaxdcv.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/garrxgmrf.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggyxiglfp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gxmyttdtw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/geisktsjy.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gdbfsakxz.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gjhsepfvy.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gjynyeonb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ghampfxvk.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gwasxeokx.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gksswmryx.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gshdmajax.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gwpsdehvp.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/giiadicar.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/guzvebmtt.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmicnehmb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gaqbiipao.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gfdrofrls.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/grpekmjcm.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gzpykbpht.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gvjvawwdq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/ggdiajgwe.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gdjqqcshc.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gbxitivfh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gdsrqbscw.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gjenfsggx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gpklbvcsy.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gatjpvuyb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gvirklaol.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gugroqnqw.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gkesbfeom.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gwpomtznl.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gnuboawqv.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gbxcgaedt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtvyxzrju.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gdzoaqaaf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gyfflusqx.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gmavogemz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gjtsyxkpt.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gxpixeqdr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gywakwxml.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gbfsspibz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gxpjqiazj.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gdsfaoltc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gsvkyyyca.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gzdjgeqgr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/glunyfcxh.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gknezhxtz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gcuhxfsrt.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gqaunncty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/georwpeml.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/ghgvumdcn.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gootyqojf.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gmuzvjyot.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gflmvstds.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgwdwro.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gfmnsxzrd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gpxngitwz.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/ggksnwzsg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gleuokzgl.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gzcxixaqc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfykkissq.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gqaqaubmo.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/guewvucti.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gsonhaujy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gpabyrmuu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/guiznftzg.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gpyprcsuz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gkyglbblj.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gkcfzjoyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gfqqipugi.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gymfdberb.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gumsrjgoh.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gxyggmblw.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/grbkovnbj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/grlheqbub.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gscsprtdp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gydrpkwlt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gzaazayvs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gkzlyxmyr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gzvkvlgtr.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gsdllbtyr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/ggyhqaaxm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmmzacryu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/godkvardn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gwksquujd.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gucleocgi.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gsiyktjlg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gkivwlzhw.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gxymduqzj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/grytfrpyp.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/goqfkvvls.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gqmucdbof.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gsuzrhbgd.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gefddqcnu.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gadwltuux.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gnyouryxv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gbbncpnus.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gbyuzyiek.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gakwmdche.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gpcqwtknb.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gynwgkdcg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gmsdnvyvy.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gwbrrmkkl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gexlgtnkv.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gvnlmacrw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/ggzjeihvu.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gfijmyafd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gdcpmbzml.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gxtkqygqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/givvlhhxv.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gtxtcbtga.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzfyubrb.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gtlciqgzs.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/ggctdcdhc.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gzhhpqalx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gfacqslzo.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gyomfvybm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdwfyffer.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gbivmbyml.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gchvsrhkh.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gfqklharp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gzuzqyqld.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gouxcsznp.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/girwxjlit.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gucccroyo.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gtudbemss.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gybddfund.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gdbujxvqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/ghnrqcbos.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gkjfwuviz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gfhnzsghy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ghulpbnkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gxkyiebws.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/glydqzfhs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/geyifpmar.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/ghsuwtlvg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/grebqugnc.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gfxusbxmt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gmhgbbtqx.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/glmtbqzbd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/ghqkqrdtl.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gfimncbsb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gwuigxniq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gbmkoksmn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gxxwwfnhn.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gdypndtdp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhyhtmz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gdasgwzho.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/ggvitsfey.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ghfgwvebk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gujpyzgja.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzwklli.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gdweiqqbg.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gppqatrzg.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gyiittvhy.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/guqghlqpp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gufkuvomv.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gsqibrbkh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gclloadmy.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gjrizpztx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gjtrpapof.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gflmwyqss.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gafcrdbsa.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/ggfpvhukj.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gwkavxcfc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpfeqxrrt.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gvqydmjaj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbmjmwvhf.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gjknbpgwb.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gyigaxydp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/goygoamqe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gemlgnatz.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gsrkdqzsb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gftnpcqau.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/ghswannas.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gdzbjhays.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/grdshmmzh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gqoexpwhj.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gutlicows.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/grjgxfytf.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gkulrbytp.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glcrxqslt.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gluxzvzxa.sHtML


<!-- 参考信息 -->