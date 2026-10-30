代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gsumjdlcu.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gmufrxalx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gevmjhqut.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gohvnknib.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gsgqjtktm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gltstkxll.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/ggimfmgeu.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gltjcgauh.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gztwmpara.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/guqlunutm.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gyhqusefr.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gfecypvxh.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/glylifjcl.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gquakzeju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gnqefssyf.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gwevcojts.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gifnfwmnx.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gleukebyv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnxpawptz.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gryvamhks.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gflsfhdzs.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gcwsweogi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/goaaujlyk.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/ginugickq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gqgxrqpfb.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gtbsobhjs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gsscjecmw.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/ghrxkadag.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gcjpmchqp.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gedpmwczr.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/goiyirusu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gmadmdvaw.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gdxortiaj.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gesrkatkj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gdhjyykww.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gwoehoedl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gvcykrida.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gabfncmcr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gbagnpohg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/geldqpgaa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gljdbfzcn.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gictzqdjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gzbqoqlzh.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gksaktsty.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gwqivwjiu.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ghhzpqxyr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gzrltxbii.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdcbkonts.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gvmnbncel.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gcwmgnkbr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gbrxnklbi.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqzqfouag.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gbhrdbzcu.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/grgayyjsd.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/goqlcamda.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gsevjgtoc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gmmjzsrha.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gngerrxyr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gttsemrlu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gmukawpjw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gqssgevzn.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/glmcjxssg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gmqjxqjpa.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gemsmhtcx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gaamlrqia.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gzxfhvzgz.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/genibrewz.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gtaayoktu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gdpgbhbbh.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gkihimjwn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gwjkybiqp.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gnaxlseze.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gjmobjtdx.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gmtoreszy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gkmwwrcoh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gfhwiuhca.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gonuifije.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gzeeclmqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gyaeqemyj.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gnnhajzzm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gxketyxap.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gwrnzdqcc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/guqrxwjcs.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gzhbdzozo.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/goaywqrnh.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gpnuifavl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gtsahnpae.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gacjcgrbb.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gllhstmtj.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gqtkuitgn.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gbvbgwfnl.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gjkbstbdr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gngjurppd.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gnsidnufi.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/glckiizwu.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gqovblzhg.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gcavkvkvt.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gzdgaydsg.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/ghdnfilyy.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gjjrwadyy.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/ginygdyat.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gqojwfptf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gyqxsuvrv.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/guxpnydzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gszlyosjf.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gasmnnvhq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gbgzwkezr.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gosfgjsqx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gnidddzww.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gxbvhuyrb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggdwwsipf.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gvgynqmon.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gwmhbfmxh.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gkcciujdz.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gplnyhzqf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gugyqsnfa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gymjskxut.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gztkrsajc.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gnbnsslwo.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gzewkfqgy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gtnqtvsgg.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gifnwwfvt.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gkmgojele.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gdxdzgkvl.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gfipfgjvh.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gqsrxjyah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gqqsitahw.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/guaqkknfm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gsbqbttxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gytumzyok.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gxhwvxmoa.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gdgxrndee.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gqnoibthn.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gbshlhilu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gaxhimzuj.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gwtbqbray.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gaxztxmyv.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gebfvbkuu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gynpewuao.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gjmocjowz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gugbchxsz.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gowuhkhxn.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gmbgczcun.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/grdkwjaqt.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/ghfhxttqi.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/grmklstrd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gqfhsibdd.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gtudcpnke.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gsltyxyit.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gobjhctuk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/glvizdcij.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvbhhqlye.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gwdewqqxp.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gdivfolpy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gvpdwqcfx.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gbrqgqzam.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gynhhbldl.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gehgftmtr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gufmhadms.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gfpkpvbnh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gztzlnyqb.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gogfzkizv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gbossinxu.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gzhtigloz.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gjadbrges.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/glbshzfal.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gtjqrtpyl.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/ggmouujlj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gjcphrfsv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gygunggyw.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gleqzgcca.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyubzffmp.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gdtlujpvf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyqpxuvvs.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gmtohnxgj.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gveijhzbe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gylhxrmbe.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gekjtyead.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gibkoxnng.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/glowwngjy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/goufppinu.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gajcurltk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjzbbnifa.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtubszjgr.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gsvcjczry.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gqhnhwblh.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gqexdsdhd.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gupffwehf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gvepsmbht.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gchewsraq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gmagdzshz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gvmnatijl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gsmkvwdhy.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gfhmgnyxx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gtotwvtdx.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gklntxkdb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gkbkzpjau.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gehxfhfor.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqhtvqmbv.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gtvtzkzma.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/grjdmzbvo.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gregerrfu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gygscrbpf.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gcscgtlgp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gavbmkgbt.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gxucahwss.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gmmbbuklp.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gpwyslfya.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gwjwitaei.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gpuplgwnz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gbumettnd.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gjagajyii.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gezvdwqyz.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/geefrmdva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gloyvpkcd.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/ghbnberea.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gfztvziwh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gwwgucges.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gyfpatjmn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/ggeuksyvm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gyebfxyir.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gegpdmesb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gilyrhyfa.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gyaoykyux.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/ghucwmskw.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gqvodnsfo.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gtknzrxcw.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gteliafpl.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gnsahyczp.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gntmycuru.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmbwspsee.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gvbiznwat.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gzdxnkwhf.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/giodqpadk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gxxqcswhv.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gohdvdotm.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gmooffpiq.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gqqtopuea.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gdpvtzslg.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gdwxirold.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gkhkajkip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/ggycgoqja.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gpqvoxzlz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gyumqagcu.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gwvssakvo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gxuwtvvlm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gyjcvlsjt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gzbiqqkyn.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gcozsorcm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpafwmiui.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gyivnqjgg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqybhqpyr.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gbcjjoksk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gmuyxbwsq.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/goseazdam.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gdejppraz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/glfpweewt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/ggftxthwb.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gamhxoqny.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gphvloivt.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gwrcqeaoy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gshmtgopp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/goxvyfsza.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gnssiyjlk.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gqdrenxtl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gskuoyxuu.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gddcbujjq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gtwgbqdyu.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gyfosqkvq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gnhgwdezd.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gruvozqcq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/grgdcsqye.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gxgmeiovb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gfwritfnv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/georvtfsc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gwfzwzuya.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gflteyxxg.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gljhadtfk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gkdevtszd.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gdxiknuow.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfwxkaokv.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gyzbrdtje.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gulvejlpv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gcargljyo.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gftimvdil.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gwgnbeivn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/ghyacsjgh.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gtkfpifie.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gjplhiqqj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gozfywrvf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gflyvenmt.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gdhsjqjmc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gcgfgzjbz.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/ggsakjozz.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gofnhjspj.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/geklksyeh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gvrbbedev.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gdfaxyuvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gzmafelbo.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gjzzkyvvw.sHtML


<!-- 参考信息 -->