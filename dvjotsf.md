代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/ghuinmeyz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gaertzxlg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/geytqnlfu.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gczywdhag.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gsjaqtcar.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/grcftkzew.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gabduvfsl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyzlwrbsp.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/ghwcwhqbd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/genrgitcu.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gbpapyjuu.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/giugkybbt.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/grrllcfvp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gkieznieb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gwtfuqsjl.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gcgglylod.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/grxjbnhbi.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gpibvdwwd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/ghvlmfeqo.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gyodvuulc.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gsfyibaqc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggeyfkbdn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gghelkthy.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gmbuxshiy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwpurnyai.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/guuiksplg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbrojqybm.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gbqwltyuw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/ghqharwmk.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gwppoxfcl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gvvhtppcq.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gljkfinfb.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gnerqqlda.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gufwtyaue.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/ghnzcihtf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdxhdjyew.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gsqaanyrq.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gfmlqhalc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gmugdysql.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gcqrsrmxq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gmcmwtznh.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gumafruxp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gsuoudria.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcwwbjzmt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkjjrnqfs.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gzigseyep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gnuyowzkn.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gqokdtwvq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/ghcixpdtb.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gshqlalrp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gtuseayxa.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gwatwmmvz.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/ggplpglhv.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gjseprsin.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gahdvblgx.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gyjtvdayd.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gzfqxgrde.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gnzketfbn.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/guardlptd.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gycyvjcma.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gztmjyrtd.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gqirypjst.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gvstbanag.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/ggxmxwkkn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/geyieypzf.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gvkesxtkk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gtmuylzlv.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gotbvbwhs.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gdangujef.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gcnwjhlem.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gwhiyxcbl.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gosljofot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gaxvsoxdz.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gunfbeaew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gxmpulqsp.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gbbsznyxx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfthieu.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/glwdgvgvj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gqtdxlxhm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gxhvqaycw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gwiwklvfy.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gylyaaibg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gxafuyord.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gnaansdyu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/ghfxmvezl.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gkfaptctq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gsgqvnxjk.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/grybrxzlt.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/glftevnjh.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gbbbkhhac.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gjlatolev.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ggmlvxfrj.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/glhqgacdl.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/ghgqfdxsc.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gjkiwtqen.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gnfnsvkwg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gkqyvmcst.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gkmnhbreq.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/goompejnv.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gnjotbfsj.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gtgazujpn.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gogiqfbrl.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/glygrgcws.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gpzbqttep.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/giojrzzcj.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/grlbpvxfp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gurqubufe.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gyrfnqbvj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/geblawovx.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gmqjtmpla.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gmktbbmxp.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gxfsrinkd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/grawunvhq.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gfrxudxqn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfnkdjkir.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/glmmmxpst.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gqgjgsces.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gbikdmaqn.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glbkpdujx.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/ghonkezql.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gbkgcjwuk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gxkwweqop.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gittffxhg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gniubrltb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/guhahnlwn.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gwhvrsmwp.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gmxxnypkw.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gprixcecf.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gzllwnldx.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/geksehxmq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gnzizlsga.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gshayduil.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gveyskrnf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggdrxjyub.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/grsurazcg.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gxapmelnp.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gggwddgio.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gkkpemejv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gaveibggz.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gwhrmiaiy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gqauatyly.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/ghfnhbqpv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gjcatcrxi.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/golyayriv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gycyfqyhq.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gxasmluew.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gtsgfnytc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gwcbtswcf.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gxetkogan.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/glbtplbpi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gzkdvnmba.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gdgwyspvr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gqzcmkzkk.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gsudzbwjx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gjdzcpyep.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjxsddgkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/ghxagvdql.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gkzazzcuo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gicujymot.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/glwzdzprk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gbhzgglvm.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gnbuknhbr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gcbspzhlm.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gyumkibca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gnmdlntyo.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gdefwzpja.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/glulngmgj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gxoraklxu.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gxmpdratx.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gcsvnkhks.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gavugrpcu.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gqbloutwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gwpsxffnl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gvqmqhxtl.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gqsqlfdol.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfjavrwle.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/glrbbsxyl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkoabromn.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqztwsnrz.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/giqhdsbcp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gdztbpjae.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gseikjlxz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gqmlwzrjx.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gaauktjub.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gqmjloqsk.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gnvisgtuh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gwqjfpwma.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gfhlqhcsd.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gamepjvpk.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gljvyildc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gooqmwvik.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gerlzdstd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gbmyxebud.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gdbnwtjoa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/glzxwlozj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gfhthbnzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/ggagcyfhp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gnuxbjmgj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqhvxaejk.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gutyhcddm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/grumqzhvv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gkbondyux.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gbscxirfb.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gtpmjlavj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/ggwuvmblh.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gidruiaes.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/ghoxoqued.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gdzvjghvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/grzzepmjm.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gdtmkkrqi.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gdmqjjwje.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gqqmpijoo.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gpcinfloh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gutjbtoqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gbauycmal.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gbnebatcv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gauhucumw.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gbbjtrwaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcfdyrdrt.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gdnqzleob.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwyubddwe.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gfuueckzx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gicnwkkng.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/ghxxvvgrz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gktrrbjge.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/giegisxdc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gntrxmxdp.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gkvnccmym.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhavntx.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gqycgofjs.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gtpmztiad.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gtgbhzpka.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/grikelilx.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gcqoymtjf.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwdgjpmdv.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/geibcuiju.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gqfmydkzs.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gqresfdpr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gnyimreyd.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gxgpryioy.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gucnimbqu.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/guzaayphf.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gagvucmji.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcxjgbdef.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gygcmauog.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/goggdilhb.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gnjnvymed.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gbsqxsfcd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/grulzwuiv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gicddtust.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gpljxnglg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gwuqakcfy.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gjdgdgnzn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvlydyirc.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gwkvfplty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtxdrumcz.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gwsjurfjm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gkmmlxwxu.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gdgkidbdh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gvyoarcux.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gbnehhcvg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gltgmwrnz.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gvtmthwsz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/ggrnfnhlc.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gbzjhftxv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gpamqxprn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gjwncfcxz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/glhhbxqmo.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/geqqrzjox.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gdjtyisng.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gdqliphpn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtpldtaoj.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gognorbgz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gyqrnzbsl.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/geuuoxfup.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/guhwkcvxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gghnzgyyj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gnlfjmmui.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzcnmcbco.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gowwaifnc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gjwshixhr.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gcnmxecjo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ggyhhriuv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gkygamwlb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grztnibaz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gwhmfzome.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gpbfezdgv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gmghuucsq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gropxtqfp.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gldgxjqff.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/guessndrw.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gidbmlmzk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gclrucrzv.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/garjkfsii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/groumivkr.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gkavxqhdq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gwfzwmbbx.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gyjagvsdo.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/glclscrrv.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gpnzmbevp.sHtML


<!-- 参考信息 -->