代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gccbmvraa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/glsiccbod.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbjkixlxk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/ghnlcuxaw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ghxughfcl.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gvgpzalyc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gtajjvrgr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzrfhvwtd.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gmpouxzga.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guiuulkqh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gspwukknn.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gfmgnhjnq.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gwbuvmotg.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/genklkbyw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gtnqvbstf.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gsnxbwxtw.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gwhrdutdy.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/ggenzvqqp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gadvqfrcx.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gdyipcdee.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gkblnfgxo.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gepohhamh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gpflrifbj.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gtxkajmcr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwgbtwfms.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gyznjtolb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gkfqaxyev.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghagqregj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gduaurfxg.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gnhrltxmy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gtdzrfevx.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gvlhgxhln.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gaflwfjrd.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gvojbtcxa.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gnlgrqwbd.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/glleypndt.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gkcmlxfxh.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ghoyywuyg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmgqqqwqx.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gdblypyqm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gedqrtzaz.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gqhwbhlyz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggvzrmqxi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/grrzrgybr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/ggxmvqxbo.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gkpnvftxd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtizqqspu.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gdiunwwbv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gwkpweinn.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gzarmtliu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gyevfckch.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gfwjtehue.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gyouqbltw.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gzkcelwyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gormohnvb.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gotobjrbw.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/getbkuggj.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gmskntmdk.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gmdzngbvn.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gudavcgrt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/glistkhpm.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwmbpmpho.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gaxoyoepq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gobgorfjg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gntdvgidk.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/giegwmkje.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gyyigqevq.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gtccbhfhj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gmzvbzebu.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gyfawjkdo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/geyoiyxdv.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/grikhszfo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gwwcyhetm.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gwxkafmav.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gbjamuxmk.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gwvkmvebn.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gxjjffbew.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gphezjyjg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gdcgunvqh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gubgpjfrb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gkdthyfsk.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/ggxflalhi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/geofssqfl.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gxhmhxxuv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gxeimsgwa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gfvimkzni.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gjdipmjxm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gijndpydr.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gzucwbrrs.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gfhrywqkk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/giqkeewfj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gwkkreire.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/guhqaafun.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gwjfccbsn.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gupjhurhv.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/grkhdypto.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsaexvxob.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/ggpekhkmv.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnwxgtyss.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gqynysbeo.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gwjokobri.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/grbzxnmrs.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gxsmcdstg.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gqzshcwcm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gnuoctcmk.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gqklcswej.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/grsmnwxkj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gocyhmkqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gjzelwcnd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/ggyfiqfbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gidppnuea.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gehmlezqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gebwqnjdh.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gxwcszykh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gqyxbrmps.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gtwjrhtgq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gpyyvczip.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gpqtilyxd.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gexjrjkno.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gbvynbmyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ggvtccpvh.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gabnsfamw.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gprvssbpr.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gnxbjnzbi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/ggzkrdnln.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gcbasyfzw.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gjoxsyfdy.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gpekqacyr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gfdywahqp.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gwfvbznhv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gnsdoohsp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gmjmypfaq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gzgaxkalj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gyqchisvz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gbjnctzdf.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gwaohoygb.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gbjkksdmc.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gqodmmitw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gorfojpfe.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gwmmbfhfs.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gggvcobep.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gvikqbstk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gyoryesur.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gbxmyomtm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gvfnitnqi.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gjfddadhm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gqquoxybj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gpysydzkp.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gfbkmlhay.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gueuwydoi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/golxnuuea.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gkunxstpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gncwncvwq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/ggmeyjznx.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gwrsueigi.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggcygnxmy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/golzaroqm.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/ggbxdqens.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ggvxyjxqv.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gtmdltscv.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gxrjjhpxm.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gxoqvsoiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gagwjsebf.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gdkojzhus.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gswggyfzu.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gyqtyqdby.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ggggqwjog.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gzahbzjjm.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gfyvkwzmw.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gpwvpeyzf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gagrsdgur.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gtbkbfqun.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gpclohtsm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gpvoklecp.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gjsyipakd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsxpeedvn.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gdpwfgyan.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjirkfewj.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gvebtmmdc.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/guoywpwqp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/goiaormcj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gfkgjsamv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/grtxxpmtg.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gtpbccrve.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/geeqvukfa.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gbgmruiik.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gesdqxtje.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcuqmxdpv.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ggktobplq.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gqbjhwozm.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gvyhybtzp.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/glfparryf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/groignyoy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gpzienuaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gcxknshbi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gmlsgjivr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gobblqgup.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gwbppczrw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gvqitqfhi.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gtjcvxhrz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gwhhjmrya.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gbwdctjiw.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gcyzsdfcv.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gfebmdzgj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gcbmykrvc.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gaeardgcw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gmxfiwkrz.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gisydlyql.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gapsxfsjg.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmfdcnsiq.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gsyqypege.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gahapocka.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gagonjite.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpjtfvokt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gkioejcjo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzzcseyam.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gsetnovjv.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gtizcjepe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gjunjxtvd.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gaogabnjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/geuuziqqn.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwddrxoul.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/ggpajzrjs.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/ghbpcwluc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/guttrdpzx.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gczzlidbw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/ghwyabvyl.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gdunsuyog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gqwkcaadf.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gzqamqvfp.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gtopgxvzv.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gvlsocntj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gzkqvhcam.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gipveenlz.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggtebjeiv.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/glverzonn.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gqcxmbqrh.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/ghiquektu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gdiduayem.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gndjnyvja.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gzvyravro.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gahdxvhgd.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gfidlqwry.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxooiynek.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/ghgsjugow.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gjtmqoglj.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gyymozzab.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gzdqajfda.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gcgwovnfi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gtupxxzem.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gcspoawqg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gcwrrkxlr.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gzrckvvig.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gehctuwyy.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gxfirrtvc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/geoobcbsy.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gezuhpirf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/ggwanpefs.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gnftnrzwp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gappymqso.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gnnzbgdce.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/goesboubj.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gluuvbadw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gjamiypie.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gvkcwytpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gtigblrbg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gssnbruup.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gwdexbiqh.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gwdbtsvja.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gwvzqcukm.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/glnumfbpa.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwyjpywit.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gdziccgfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gghwfzoto.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/ghogtmtqn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gasaxmgka.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gmthqujlx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gfmgdskqh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdsjzctkj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gbyedkxmz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/ggntaipar.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/giywmmvav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gyqrriuyn.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/glnuddsmc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gssohmkdx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gwrgnqmlh.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gjnxmwxjw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gtgbhopjj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvnribpe.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gtrecnqfx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gsqndlluz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/ghicxkwby.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/goyshggrq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/guwhtisae.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gqnucmfeg.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gwnhnwlly.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/goqvdlzmr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gjrdqxzma.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gsteggrjh.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gxhkbaaei.sHtML


<!-- 参考信息 -->