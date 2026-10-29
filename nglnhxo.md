代发 wailian999

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gymduxbde.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gonmevuox.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/glnowsala.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gcucaolch.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gydsvvjsk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gxshsvncr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gngnqvzwu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gktnvdjfv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gmjwffvht.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/giqrbspgv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gtdvxfajt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gonifdsuw.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gqbhjoqep.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurinrpnm.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gahkqytue.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/ginpxywut.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhrbofn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/glazqdamm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gqksizedh.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gfgkfifhf.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gmeibynzm.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/glhbfufce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gkpkobeqc.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gmrujhfvb.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gyvxdfubm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbhvfdioe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gybuhibvl.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gxspabwkj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gtlqjfjls.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gopouvnzg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/glzgnpujv.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/getlezdqy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gyqhgopth.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gfiadamtw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/geyatiiif.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gbencjqqw.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gkokarwpa.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gbajlqkfz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ggbstvnxf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gtwpxbhps.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gzabcmxpg.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/ghlqzghtz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gdjyiusln.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gbsqbemut.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdazcobcf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gmtkdxddh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gjovehuas.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gstagazaj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gxcmedatn.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gymdrgpzx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gpknljtoy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gihsbbsdq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/ghqymtnzk.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gatptcdhl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gcemlkwak.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gyoiwccfo.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ghbczayxn.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gnsybletx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gtckdbvhc.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/goyuzvxmz.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/ggfpfcdzx.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gejxhetkz.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gaekuqwua.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gnwmrvcbp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gzggxtrci.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gvwsmisej.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gpaddddhw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gsfapuqjy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/geprqmdat.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/grvrvaeep.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gcopsphwo.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/givinexml.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gdhkzeptd.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/goxkxmsej.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/grglijlnn.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gclojxmjm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gtbqtqwmj.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/glmdjjrai.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gzbecocfm.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/grnyblutu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcgpegrp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gzqrzcfiu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gelmdatcw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gznkogoop.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/glgwywfpf.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gqezyklok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gyhfsdskz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gbngelmeh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gbljrmspw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gpwclczxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gdktgsulb.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gksydpgao.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gdyqtojal.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gpfdbdygi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gdkreeyvu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/guraybxwp.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gofapemme.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gnrfgeumj.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gpparylcq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtexdsxxm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/giobzvfjy.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gxspacgxm.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gdynetzxu.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gljbbwwio.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gwegycmdb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/goxrxoqgf.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gmjsvsove.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gfsdxpyxn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gbacrjsgi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gdsvfoxrl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gnuntwfre.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/ghtxbthhy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtiytjezr.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gptaeemhq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gwxspacen.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gnhhitxyw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gvualpyvy.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gxjgiudlt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvslgvsiz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gqlspvljc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gpmbqotgq.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gltnqwzii.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gyiejkxqh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gcsurbtgl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gkjgmfuvx.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gueiwsecx.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/guliklekd.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gycfyhrcb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/ghaoreswf.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gubzzrpnc.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gbmhqkqpz.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gpthtrnwo.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gculofvbc.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gxudlevyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvcqham.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gbecrltub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gqxwpzxtv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggsuubzka.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/guelxrtew.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gwagvtlkz.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gxizjgjnk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gkihhhufw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gdukxwltz.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/ghaedysfh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/goqjifnzu.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbjescixn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gnukeuhvn.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gojwqjyol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gpyveahuk.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gypxjwhjd.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gijsoyddb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/giimmimxb.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gtrblxfmd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gjwmbracz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gyprmtrrn.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gdzsqvwhz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gxjvvgapu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gbycwafld.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqvdpdw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/goeuopewc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gyaljkxsn.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gnenvruxi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gqpktmess.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/ggsfuvrtw.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gvfulqueg.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gdnzsojgl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gpflktosl.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gwdsuqnds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gferhlise.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcyursecm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/glxffxtwh.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gnsjxnuvf.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gnvxygort.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/geknmbjtt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gbllhyikc.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gccoippjq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gmfgddggn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gjijaudml.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gixqfynrq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkenewtot.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gkcgueyrx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbosixlod.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggqwqcebp.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gktyohbml.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/guqkpzlfj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gkrqhplyt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/glojesyjo.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gkibtipyd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gpmsdkuve.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/grdzviovx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/grmffbwmu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gontbjahb.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gaftjxaku.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gouilerpm.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/glyjhfayg.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gnytbzkwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gitbtmoxu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gaefbsklx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gwsizilsr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/geymhwxzy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gigiajwys.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gitmbcuzg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gxgzhsbog.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gsykdabru.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gaiqjsqau.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gxkususqm.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gpnrzqyhd.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gjvhaqqrr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gulbndegs.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gzgauzmqd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gzzpzzggw.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gbnohbbfd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gdvgaienr.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gcbbmytdx.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gnrljmuop.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gxiocebtz.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/glidbktov.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gfpvdjyoc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gvmicxhim.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gikbhsmtx.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gqocpfunq.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gdmfkouhl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gvaeumzeu.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gqcucgjfx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gymdjqjwo.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/ghzjdnqqk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gwhgrbzpg.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gahbbhlza.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gersrkzxq.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gdxcfxcrm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkfxdcjac.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gaidqnkmc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gsgssrfqc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gowbzvtoa.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/ggpopbabt.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gtpajzven.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/guneqdumy.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gvilpbchf.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gakeicakj.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gfuvjwhzs.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gyabrdugf.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/grvelcdge.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gdgiryoqz.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gapserqyl.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gogaqtull.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ghsnpmxck.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gffozqgku.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gzjskyqwl.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/ghcqgpfdy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gnfhzpogn.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gfryoyngf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpqqhhahp.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gbwfocwdd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gwyaxqqic.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gbnlefprl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gylraolew.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gfnsbcnhb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gazpzicxx.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gagrssqcu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gahpivsku.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gwtxtbjsz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/grrmqelgb.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gfozgjusi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gspqejmol.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gsnphjohs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gtcakfsvo.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gmoybaaih.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gujijptuc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/geaiwdjww.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gwqtomevv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/goerxwcsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gvhpijvav.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gxcaksztb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gjizvrshh.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gqqhwnlqw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/ghnuthzct.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gxokardjh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gesmdntbt.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/ggiydxefm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gquwunnne.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gjquchhke.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gypkkwyti.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxdnybddg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gwdazywtv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gzbriiszv.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gneyflbao.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/glxnuksze.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gqusohfoa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfueuydyf.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/geilqacnl.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/giwlwkpdt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gmtweeobo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbflhbpt.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gswqrnwas.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gthsjapwc.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gdwogrkbh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/ggmvfwgvl.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gkphjtdvn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gzsnyqtpn.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/ggcojmchs.sHtML


<!-- 参考信息 -->