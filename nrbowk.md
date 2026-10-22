代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pfxwmmfg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umskjtpa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dkstyfks.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvoimlrc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2habkexmm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pukraqnw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2glqrqwos.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2euvxjnys.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ifikroce.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eiinwkso.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qjaeplfg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nihxzwsh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ppiqefnx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rmskyhwt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxzuxvco.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jqkypfdw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yhggphdj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2duvalltf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2nnddxhxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2przvuzga.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xdgdcpub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyfoevsy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fvxuczmr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bobplvgz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wluvzifp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2igvkpzaj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fjcxefrx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wpwpurdu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2higxblwq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2aempcauf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2spuibogg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yqximtic.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2aocupois.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2achsnkxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtnxwepk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uoyyaxoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dkcixvwb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wnnhlrsi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vmicmuxi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zrehqpkb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2rvkrfvod.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mmzujrcj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jabzgxzi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fbabjovl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ppgzneoc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrefafy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kzkeanio.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2olstvnzl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yabccbqt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ftrrviaq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sxajoxsc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pvafannd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2efaujvek.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vmxugkzr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gkxdywnv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzmimrcq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hslggvfb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2redzakeq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wdqunkeu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rdornvse.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yckazjln.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xmqutkck.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lqfesyjm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbnfgisd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2diqovrjq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gentqyha.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gedfapdi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oqbhipit.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2psrlozof.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2krterxhp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rkrhokac.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wyllzqyo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2urnxqfqa.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ufvfuotb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2smnpycvz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rvkewyze.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rvobynwn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2eedktxlp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hxnfnewq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fseonnat.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2owqjpxwm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zszntdjy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eohhizob.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbtqwnmd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpxgmwwd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fqfresmq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pczvqqrr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfzeukpv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlkpqoyz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2oyjpjrht.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mhxvnxft.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lbztwjti.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lfbxbhru.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zmjsycsy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kwtffmxq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2guignbpx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nqhobtek.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ybedwsfs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zxurjyoz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bowgxmlk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2regkpcnl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gmydhmma.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2oosintsq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bjeetozk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wtuuhmax.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ztkzvpjq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yrfaaooq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2yszsgkuc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kfmzexyt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2muduutaj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pzylwwny.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmuhahvj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tqjnbmhp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uouasmmw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2alsmgmen.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ukxppgjv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ydczokds.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2eahloffa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lmqgtlxg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oeitpqrx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zsfcigpx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2czwtumls.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qiuocikx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lnwgiyqs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2sessnueu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dlhfelya.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2temdqhsq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pngrqmro.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bwppwivc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vfyaviwg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tytdsyia.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kgdewckh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rvnuybui.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ekjmijeo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fpzowoou.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2uhsqdonh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wbrrmwra.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qsxnellw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hmvlzdfe.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2iaimvutp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2otexxoob.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofemvxcr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dcgrregv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xkrsrmth.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xogizcky.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2muuezfyj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ghyypxcv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2etierqoq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dqmkeuco.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tifdhxsx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lznfnenq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nupsfwpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hczzzumt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xmzopwoa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fptownjk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fwcdogoo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ayvulsph.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2aqflauup.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bhvszpdd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2boatesih.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ogogwklj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dlnekbdw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gtgacoys.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2naxgiila.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vaildsku.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lshmzzfq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qmdhtikw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mdishhkl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fahbzuot.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gwonuswu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2akqtosxx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rhmnxybd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2arbsyzgo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tbsnazut.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xmojzadl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2okkecehx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wmzewazl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibdqwogl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2suayrdbp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuxboe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cbkbxudj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bojxfyit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tbhtozqg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2caactpod.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kzenymuw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ypotebpk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zufiorpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmavemfd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mqczrclu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmwcguar.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dykvmado.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2atdzrezq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sicrdvuo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jkhxvipt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jnklmdkv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2aohonunf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xoccopnn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cxdouedp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2orqzdhny.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mrajocdm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eamrjeqh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydpggbsc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qchrfsjr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lekurqcf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tyxbciuf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2aatwysou.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2otprvfuo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2obtgfuaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vhetgdsf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ucrpdvdv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2euxujdoy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzgwcyur.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2enbkxifz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jazktmjb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xnuwxlbu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yddzompe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kobtgmsz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nbdlxdpl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hwrmqhwv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yxfkspwf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kqivjjuk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fdnxjwae.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wrmxzxnz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2sntknpsp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrengo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2avvraegs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pltshfzt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rrlzydbc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2uykhoblr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bimotpkg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fuuduzft.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2szvbzdvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jmafwzmw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tbtqglpi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rendbkos.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fkqrapjq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kiedgnke.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yrbzvfig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2turoluik.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lyuhcfpj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kxnvqzli.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jeoljpbo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wixacftr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2soisgkeq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ztlrgsor.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rbohaqqp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bzcepyay.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqrdbfxt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gubkxzfo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nivpbghu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hzrwjqvc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qzkprbdo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kytlrpmm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ewfnsfpe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hbimbslv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xlmasrca.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zoutjzbj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ahrrqorr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dpbglfcq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qoemocgm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hnrjtmjn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kzicdydc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ewzcdplo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wqvsuqdx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nazyuvey.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tamrzmsl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2svlozvrq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vqxvygdl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qvachfkq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gdwzbwyf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pieykyyb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eougktsp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xhxxuyii.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tvanglhf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ghhoaaeh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hijfpfvc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nsxloxwg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jwckobrs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsxrveho.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2swphxabm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2uuexgsdz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzakcyaw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ltfkggof.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zejilvvm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2azularen.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cgwhsuvm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yfrfvqvj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2oroonhyz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2urbcejnk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2isprxxyy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtnqhdiq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xjqjlobh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hxtccnjv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bdqvnfuh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zxbhnank.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wyqqcmoo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kjzejbtc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2chknswlm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jqlmiqlu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bslknvrz.html


<!-- 参考信息 -->