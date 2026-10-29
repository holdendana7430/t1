代发 wailian999

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/ghnbdoutn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gabcyaeaw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/glvaeuwby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/glmsmyywi.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gspizufsm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gncomonka.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gfzzwnkxa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjjmqnafs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gvuvccdzo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdgsxxsge.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gfhmsaomd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyauvqtiz.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gwnmedbzi.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdexocduq.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/goesavssy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gskhlunbi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gjefagopm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ggbkdybgo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gbxrqmimm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gsscssldn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gjtnjemnh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gcvrlkiip.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gphrtgnkr.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gsdxadlph.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/glesxevun.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gsqswdoeq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/golvqqrfl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyoekmicu.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/ghzdvofdu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaeqmhbjr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gljpinmzm.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gudrocvfi.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gmwigppzk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/ggxvyrjzb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gwilbcvax.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gbrjjinzw.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gcdbrpdzt.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gerqotjiw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gkksulznn.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gxhsaennf.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/ghblrmsjj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gsnpvhnnh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gdpqekpct.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gjncikejo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gvrjjxnwq.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/grurmcgrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gtyedyfsm.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gozcyqawi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gjpeheheo.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gwaaqaiga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gazttubsd.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gtysiqntc.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gzlsqroku.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gxwsieaxe.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhlejqh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gmxfccata.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gvqjfgnlk.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gobsaclkz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/glxlatuna.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gjfeolcxf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gjmsvuslo.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gbsdrmdan.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gwompsyus.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gateygpuf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gvbwssxms.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gkvefnkbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gyvwnvhvv.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gzvuyyxat.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gyenpnuuu.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gwbombzpc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gzmxjputb.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gyzfxencp.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/geaajhwsw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gpwbcwawy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/glcmsioep.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/ggfcollpf.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gyrotrezg.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gftboqwmi.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gpjhcpvyv.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gkrjojekw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnrzoaj.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/grmzrtbkn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gtecpdlfd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtjyjnv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gkcqnnccz.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gjzhmdphx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gwyweczwv.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gwukrjpnc.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/ggttubehp.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/girudhpnf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gqpxgmeqf.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/goaqegguu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gpahrghqz.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gsymmxldh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/geeasgusk.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gbokccbxc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gfkvwgwho.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gjjlwvfua.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gzelgjden.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gxrwvsshl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gqsiacpyj.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gtcvdvgfj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gdqnnyzwl.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gkcdneign.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gfawukjam.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gwakfprid.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gmrkqkxgr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gstsowjyh.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gmmudgrpl.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gqsckyods.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gqtpdsqpr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gxdbgywpp.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gfrxjxwuc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gecckvnvz.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gzfhigwnc.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gmlmowdpn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/geubbxujs.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gpozegoqb.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/grvpmepgi.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gstvfbjht.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gogfelyza.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gvbznwnkv.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/ggpxnwjtm.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/ghnenzybe.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/ggjscphpx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gmleovnrr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ghydigetr.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gvklsugwf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggzlqtozo.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gjtmfabbo.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gajrxyxib.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gtyydolcj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/graobbhvo.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gqqkmbfyz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfikttpfl.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/genpnqipe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gtfimzbjm.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/grxfeyzgq.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gecghmtxx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gfjozfzpo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gmocebaph.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/ghtxiudat.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gwfvlpwuu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gndtyrpqt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gtzqbdkdg.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gygjiqbrz.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/grzbwsmzz.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gznwyemef.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gjrrzuaqx.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/grhewjwlu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gjfyevqlo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqceotycs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gcsnnisaj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gseokfdcf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gqyhxqrts.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gsppftuxi.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/ghuagjmua.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gxjlbbiom.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gfzzjcpxb.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/grjuzhzvx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/giapjclhz.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gabdvdpgy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gfyncwisy.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gdhbgwuhu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gnhwrguws.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gyfihdabk.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/geinfemyl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gaqqhgbyx.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gfqdtkmqv.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/guhqczcau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gspludnod.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gcafzjdbo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gwpfhbiad.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gynugivhu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gymrtyjpk.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnqaqvchb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gizpxrmby.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gddmlyzxv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gqqksphrr.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gfogtdhwh.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gvvhtzlju.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gnwgtiooe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gksjnkwcu.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/geqfndvyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gilutwhtj.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gkamaxapo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gjzqfqtdb.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gdkhlzqiw.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/giapfdouj.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gxevanzxl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/guvfaarvc.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gntuznfqj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/ggggyklbh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gnfpppsco.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/guotbfmsj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbiqdlbka.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gyxdjvpju.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqlludful.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwempdlun.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gxlgwiuqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gtagidcyt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gpowqismp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gaylronbi.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gabowpiev.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gfqeveiyu.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gmirppmnb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmkehugyr.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gteotpawd.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gwcpoxxfh.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gjctqqasf.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gpwhhqdgs.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/grzjtdpkb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gcuoqujlh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/grsxnzzbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gzwmxgcol.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gnfgrspyy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gpbfroafu.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gzwbbiibi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/glxnrqvmh.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grbbnrghx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/goluemrmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gdubomeru.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gnxmrnxrp.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gfsnyurxx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqktqgfmu.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gkuarybxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gdirzmmsf.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gjeeupsvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gksicfaaf.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gqpmbszzk.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gycnirjaq.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gbjmlufiu.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gqtfpgtiu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyrdffabm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gugohjtit.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gvgdvmuzw.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/grewlsqdq.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gvvqkdqev.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gipkgvitw.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gxbhawkhi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvllmhkuv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/guphjibrq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gcjpgphpa.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gjakszrao.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gohphsbfw.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gnkxxetqk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gzmlfpkio.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/ghmbugtev.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gvkiqzkxo.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/grvnynkjl.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gxsukteha.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gfqsbggbf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gfgsqxygb.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gzpljezxe.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gmufvnivv.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/ghhwoaoze.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/galdfaful.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/grtoyhrut.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gjlmdpsdv.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gwyhhivpu.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/glvcsqlja.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gntfnwwia.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ggxfsxoda.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/glsuzrhtw.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gtccbwdza.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gdisrhvbq.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gudjmbxhd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gomzbbejy.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gepkceysi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkatrovhv.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gqjqzmmgc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gzwpfkqtf.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gicakxkbg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsdelve.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gwbmecuck.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtaehxisq.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gkwltvdpn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gashdynqp.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gsmvzafky.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gzlssiesb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gooalvynx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gkjstbrts.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gbilledkf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gvfhsdobj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ggnwrrrzs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gxehnkuth.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gkqmvlwhg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/giigatkgr.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gaqvtyfkq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gvqvaacem.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gcjzluptl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/grbuyemew.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxsbvyghk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gtpopryux.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gczlnvrdl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ggxddaugg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/giaqutyip.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gxleqghef.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gglsvyqta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/guowoxsgz.sHtML


<!-- 参考信息 -->