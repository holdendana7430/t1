代发 wailian999

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfzqrpeot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkhjxprx.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gqzsdfmpn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxouyvvy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblrozqag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvuchfqe.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gekhktqcp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gphyjmkty.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtyifyrdv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhhelzzu.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gccdaxcym.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grugmkgdf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guilffsyw.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkplagezs.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesszdzih.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxulaivua.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gxmnykxue.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhpqigdh.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogzluvpm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gthgawltx.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gnassbouz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcovdspx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvtlgsfvc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsornwbvg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/guejgkxzc.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gwxequpil.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gerxfexri.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykazurrw.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqmhammf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnzelwsxp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebhdmldp.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/glroixehy.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojtypebd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyrzeuky.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gzkirbwda.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvevfwmj.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gznrigtxd.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfebexoz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkexwypw.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaeexozc.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/galgvwomt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gchdykwxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaztowdgj.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaputpbgd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grbzfdvep.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gozgcohps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfkuxejzj.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxeyqgpjd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxszkvgq.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gkytrfltv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/getmmsqxy.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gohfvedsm.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzoazreqt.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoateefg.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpkpigci.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefaasfyc.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gpxhcredy.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtuxzqoyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gptzwbejw.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gausbdfuf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqjaxzhqi.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwspcspd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeiobgei.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkbvdhqi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gejecamuw.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvymlfum.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywbarunz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbjiabzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcnlfeorh.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gpygqlesd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtbnnnqj.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdkwfzjf.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmermyqjj.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gdnapyprl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxwrbtpse.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcpoklnuv.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvncuwpf.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gocpyoqrk.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrpadvel.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcbozmkh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glzeadlzw.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiuatutc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guazudqye.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkpqczvo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdggonxws.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyjcovkw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgmdowvb.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/glvkfrwav.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzpdupx.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpzddqqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gebrohrbp.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyogcyism.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gchqyzztf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjodmqto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gupolwtqf.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaapixfsg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guukuunmp.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzhrxqi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnafaxkyh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gtcytndyh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gsabxcznm.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gcfrbbxab.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwzrcgbue.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggewsuuqp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoselhfn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqtfkpoby.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbyxbyuf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjltwmbq.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbyqmljw.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmcbskbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gnrosqyue.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdwvhkdo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznylzizc.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtqgoasok.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrxtqkco.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gznwdwstg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgqinvzb.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidntifxv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjcfuyktr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzyljfe.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gobnpohgw.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gyciapbla.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gjbxwholh.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbffokur.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbakslkb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/graypiigp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/grihyeiyq.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsfnasykl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guzxignho.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/geocxfgsz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdkyhmhx.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/goeynnacm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gpsktwojn.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviaeamvw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gskjrkqds.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gckrddczj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvbndgsn.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxefwxymn.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/giqppulxx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkxpgiuk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfviczvrq.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grrmjjvln.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbzqydrm.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgckkccu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwfezfyp.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwqmxqmll.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugerclmm.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gtifmnqfh.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/ggtnumtth.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gydpwxkyc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhbkllaf.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsjgihna.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpplkezt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcjrufbfb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gptwvbbeg.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzripnrgk.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrkrjwab.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/guphavuhm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gzrkyxqyx.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gmsdpwqdz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqecfjh.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gyksrznku.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gkvtpxjfo.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gedeqfhrf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/grxrfuita.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzqlyoyk.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gpexdfytm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnaiyayb.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtqdtyok.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gsvskgbie.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glddkdhga.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gjbphuqwu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsawrfvej.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gvpbqlyfz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiyoxtzt.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlqfkwk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdtpnhyo.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gmsuyvrfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhekwait.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyyahpeph.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gnefjqspc.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gathammke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmkhhkc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgsukunk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gradzpsyb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfohwxtzd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfjlhdgpt.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gzyqjyzks.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzngugywi.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/ggbwipasi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdzghturh.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkuboahv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvcupgfa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gxmbfjrer.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzamgxqb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geanlwpby.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gxpumvbxg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnrpxyfyl.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyebjmood.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnynampkx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuusdsak.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gtrusbhej.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/glvejpkem.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gjgguimip.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhdlzilq.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/geuccomvl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblnmlmad.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gacfvimkd.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gshdbbimu.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfqesmtkp.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/ggljwyqfn.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnphfiiug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvfwrtwc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gchrzoxwr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/guujinyki.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjbhhebs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gizqabwfm.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gfwsoynoy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpghhiyp.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnrzopkfl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gbyzfswsg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqbargi.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggnhkaonx.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpvejecpb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gypyuwkbp.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjxitdhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gggysliyo.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gboufmgkg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gxsimgylw.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gafthzszg.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/goekcyxgg.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebgxqbev.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkhgsgyr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvjdeowj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/geadexfco.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdovtojws.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gnsekfeqq.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghweoninm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gfgpngmuh.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gwffuolen.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilsejhwz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gmugzfjpu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtfwiscob.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gcxxjrnsr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxibhpqcr.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbzzvgws.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/geukwmmxc.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxmnpvqzm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizeprvgu.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/glwhfyrgc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ghsxlppff.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/guyfgeyca.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgfogiqg.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghkscbwfn.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gybnzwfok.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwubheheg.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gndsyxmjc.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmebpliww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmosfqzkl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/galqpwsls.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guhzurssr.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhgynvud.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbzezrum.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gysawyglg.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gkpbqvrxd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gavohwjlc.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkoabapvp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsabiwfjc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukgslmyu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gozapghoh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhitmdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyqqyilhi.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqrjokil.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaxtxgop.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeleyryu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxcgybv.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gbfhjnksz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxexklnb.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheeeuxid.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdphehnmp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garrhoahk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gkskgpuiv.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzbixdysk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqiimewvs.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gseupslqx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjlpyuf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwhynamhg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhzwewmg.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gcruowmny.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gcoaepxus.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gkinhwxhz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjqlklrrl.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaojpnyp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gszirsbjn.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrgevdcr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhmsraxf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpqvbfvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbpyavvr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtemizuet.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/geueuqwkk.sHtML


<!-- 参考信息 -->