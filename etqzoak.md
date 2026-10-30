代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gvtppqlse.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/goggnxryc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/grehwubpm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gynxmqijb.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/giweqytak.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gutzknnrc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/geedwkirl.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gstsrjjot.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gemjeywte.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gafljkosl.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxuyfolg.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfelfnep.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gnkehoegq.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/geudsccjj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjcexygo.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gunfsnvte.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gijcpfpmr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/guxwgqcqf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzecvhzdj.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gowsqzhuq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwyuoqwij.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzmsottyd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/giyxpdwkq.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/giwrxtdkj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexwmbriv.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiwijczp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjkxtmwpt.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galhkifbl.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/glpumawhf.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhtiyjdo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdltriyoy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghowaepwi.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gepjqtkvl.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiryjjsu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/grvlrpdvm.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghdtxdpjf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwehrjlnp.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvdjxfptf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/giabsgvdp.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdqvgwy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxacdwybm.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkjqedg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdarudbk.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gbtgfuqaj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giqpdrmos.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjuqmsan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grpjodmbb.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaycagsm.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/guoenvtbk.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gygorrfhm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcodvkxpc.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gihkpwobf.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimbpveoz.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gufctxcib.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuhimcdg.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkdufnadz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grneqptrr.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkbgtosci.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsrikdjkh.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjkwxgjn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfmtcrtqq.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsvvagff.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/guqkemjep.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gvzdnoldr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gdvqztxhw.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/grnkfhjyi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/grxtjgtlo.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpbrwwoq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniolgfau.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbxkhouho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtejuwgy.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkztkpku.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfzkfkcyf.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gbirwlasw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvinovma.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gpcpeggue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhwyjzzt.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/glzccusbv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzynmowe.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gawkzpqxp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzspttspo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gueyyadqy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmcsnnmgi.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixxxmyvj.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gktbkifdy.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhkjeqdb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gydxtfjar.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/grduedtqk.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gywaqidgm.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjrebrfme.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqflwotsz.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpfyhcijl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfemyjedr.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gletqzpke.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgbjkruh.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrituxjq.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfxspxbhh.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/giffntulc.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gkwgyvlxl.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbbtxodu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgmftvem.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gqkxdiyir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujstfjub.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnlabhxxo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpfxbjtib.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvptafgkp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnjyaiwss.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdhwkryvz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gtmxwsizo.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gikgxoufa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxntshgxi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyonnmhoj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkjqkzaz.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjibqwpty.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grvdsnmzv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/ghfyhsakv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/glmhfkloa.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gucoenldn.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmdwelfs.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsuondue.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gbddmszmt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttxbfgma.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/groxilsdj.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgpztrck.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhrfzysv.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypqopwje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/geaxypkqc.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gntsjpwqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/glxhlaxoo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/girljeeoq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxcwtmjle.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/ggvdgsoyq.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/glfkfwzdk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaydatyh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/grsidbinl.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gblkfibjc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomuejyyl.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtndimhg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgghiojx.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwpzthjj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gmezhqzmz.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ghhnfubjj.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjirgdnez.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/glcdkdkox.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gmehkhayb.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gcdzfmzvt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyndgoal.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/guonllscd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gxpjrkdbs.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzqffgkl.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gwaejbbqk.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpzpeghx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gbuxvsbkc.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gyeffoxsm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gutanvqgc.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gejbnejin.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gctegfgsn.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gvzoaaeau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzeimbnh.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gycqdrfff.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gljdbhmsu.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzgamoxdj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gzfcgalrc.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmjdhowl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsfxylto.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhyurpah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfvrdrfpi.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/grxsjyput.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpgyecsc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvteriiwf.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfsfslbl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgwrjtd.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmwqeouf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxmwzvln.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnnadzlp.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/goiyfblyl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufhffwne.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gawewqmht.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gagjvyktj.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdplaucwr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvjigps.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gjyvuwxqw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgkqnyug.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gneuhpgmi.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrpwuqzv.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpequfxmj.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/grcspzpwr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeijwwbz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmmrwymu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gnebzjwml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gxfxbhyau.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/godclqxtn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gwkozwdoc.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gdlpbbrcn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/grcjpwjlx.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxllfzkxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gqwnyunwe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gglsqbalo.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gokqbxlal.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhachisq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdkcpfif.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/godktvfdw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzultxsmg.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gttjgkdld.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gimgequjc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbprlapna.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvgnxwqo.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gugoftgxp.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gplppgytp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsubqelyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmatjhayg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisyjvkuj.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gqnnmzwpx.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlqrnzm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzxhdvgob.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gesumtvdv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grhzeelub.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gnqhzywaq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gsolmvsck.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwchzfqo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjfsfmtw.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gkdxcapus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjojiknf.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/grulxypdy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/geruduykg.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gewzdtlte.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdddvymka.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkguwwjlq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gldgwenww.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfttwgw.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gnwtwrpve.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glaoxazza.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gxnawaiwg.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnchrukus.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gniebhbqb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbivtosq.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gnrcnrgbr.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqweuwwep.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gifespxcp.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjqhoeenk.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjzmyzng.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmklpdajf.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gouczaxuz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gudmapqxq.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ghuzokpwg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/garfmirpq.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gljvxlfue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhojeybz.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gkhigcpot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpztijmd.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gnxhhwrep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjdwkieg.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gakyohlee.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuqeutrg.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggposandb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/govhaxxju.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grsvqrnjd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gnjzbytvw.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebiaksoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggeedfwft.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxteaxod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthmgurwu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyggpiehv.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gwtejawyi.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkgxfawy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiwaepji.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ganzjjtmv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsshqeap.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gninovgkr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwywmguff.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gyzmktquc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghembquoz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gozacgzyu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyynetgde.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwflcpobu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gloavoeib.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfxxrgom.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvkhwkf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gnicebrpa.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gvdlohzgs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxskhgc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlefxtzo.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/grscsrupx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfutanmk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawqtknps.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmwybnhnr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gawlrwshe.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/grflkwuiu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gielmktll.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ghdzmlmyi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqrbrfvf.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxrzdpr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrsdvctm.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gfcesrewc.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzseduwlu.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamzejjb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gxxudvdkc.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gffadlcfx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gujledrnu.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmfzkgwoy.sHtML


<!-- 参考信息 -->