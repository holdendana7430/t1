代发 wailian999

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/guvpwvcqk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjyzfwau.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdntebt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhpiqeng.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gjgdvjlwh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsymsqyr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gajjndknq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpazndvxw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gwbrfcbwn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gtqcwwfyv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqrnwmuaq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajvsxsdc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlssnhxv.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyggsmjee.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gavwtibte.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrwfpgk.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwzedcehs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdeptwud.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/glkavdtoc.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/glumokrpn.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggurgyzmo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gxqqwjzsj.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwbtpajr.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grzqrbbof.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqifnepg.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpdcvnbg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmystgsg.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/glrurnezy.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gryfmtyvg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyquwzgln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaqtwfuy.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaalsaql.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpouuswll.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbfqwdpk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbowafepi.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgxtslkv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrqinhgq.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzarhvq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvahnhdqr.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxmuvoy.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjbglkq.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxarunhxo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtzqntjr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghczbetat.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gereidoal.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/garllgogy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gljcthkwp.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlfdlkjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gssxnxpvp.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/ggraylhss.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljypouku.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvnyxeoia.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqhtxosn.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/glricxshp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkldkixs.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffsvipwr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grooinawg.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gptqibxrz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzlvkcyt.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrgxltpd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdlvgyuy.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gdptrqbcf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjbwpnoc.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gxdczkvyb.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkmivwjzv.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhxkuuiv.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghojbwmqa.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgsjuajl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgznssvn.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdbmpufl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaelvazdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gokcohuhh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxskxkc.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/grmugsgce.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaagyrovp.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/grnvbysxl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gwdyffdpa.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukrxpxmy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyezbmav.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gniqtovbh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkalesadr.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gpoenxkbc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtotqntny.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwrcixht.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjcaxbynh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyysbdkj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpevryjkh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gseuafmwa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdhgmvzt.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvoyfbic.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdrjwcjkd.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gvijctbmi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeidukht.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluoqdoqq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gojaokukx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gedhwnywx.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdjfshvxh.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbugzrcl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgzrprys.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gckxywncr.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gohkayxgv.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsybqkce.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqldktbwj.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrdmbckm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgniuplt.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmbdczji.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtobdlag.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauqpigyc.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gxndgiips.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmedjbyml.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/giifciygk.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmaxrehqn.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gkztsbenr.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmkyqfyu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjxativo.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcwauwpu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmrmmepso.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ggdsvusoz.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwwkxoyzp.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjyimjpjb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gelndttef.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhbftmkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrvxzzxy.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gbcyrrknz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gophpfhid.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gpllamuvx.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuodbcpx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhgxsoop.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gumldhhty.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqayegcm.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqstznclf.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/goaigqhzy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gilxdpvls.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdexsnqzp.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/guildsfsb.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/geawzkoja.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/glnireujt.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwuaqya.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gsjntklsi.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gboeugcqn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmumbckz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccroxtm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwajhrjbk.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gvncqxjzv.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwhvyqit.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnnsrdka.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/glnonzxyo.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/giojhkwvf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gnkjbbnon.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gwrhhyadb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gfblmrqym.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/giwyyfvbs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwzkuxpi.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrnwweye.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwaxubxf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzqlhpfy.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtdqljlx.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghsohjryl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujerzxf.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/ghqdjjggb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdawzuuae.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grazmdjfl.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztdgigvw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstnilnvd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfezkwie.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaklskrw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqutsvhg.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbzkbbolh.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gtrpjkyru.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giybwuodr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzyilrdv.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuunjwep.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmiyeahi.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhprvtkf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gcogqcmhl.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggipmmaca.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/genhycovl.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkgovql.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxxpdnnbv.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gazcbkrrv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gicuctzoj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgrkljwh.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxmazwyg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnvvnhgd.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gdkytkgac.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihobqzsx.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqrsewsmb.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gbcsdjzep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpmsnfzuz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gieitoqum.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gydlmrcim.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwtojyoqq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiyxembs.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqavewjj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaocsfyu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqlrgxii.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gaznqsnpw.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtucxbtk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gczdeqath.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gawirpaej.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmmriotf.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gfztrvuxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdffryyqe.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrouhgds.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gsisjlyny.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdhcrdjy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gdjijtowg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunthjfkh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/grfixeitc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaavypfq.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhdxvqwv.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptmvrewo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdqypuxpj.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxuqlmmn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gcekvryod.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhwoxjjy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjgmvliq.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlprswvt.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/ggdbeiupy.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudpzdwmd.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtmhxjgy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmltdglsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqufnjoej.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxciaujv.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gdymuoyud.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/giobafbbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygkpalmq.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocfpsvpn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gfzafwrqv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqlnewdj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjnpggco.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnanpbavr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdypggkps.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcykdgckl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gpbpzkvye.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gocedwrhj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gaskneutb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjogiqzow.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtrzkybc.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwhqeqme.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gueyspyym.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gldgqntfk.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrtgyevx.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gykrahvok.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gurieebdo.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyspwxmqs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjfkppxv.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gxixaobyw.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gjqtfueso.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gapesegxv.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgjresth.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyimdmsmv.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpegzrdu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjtvbobo.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/glhmcqrvh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjtwtoxq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvxpgkqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gkxewsvqw.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/glplepcef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbsuctaj.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/govhbhzdt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggmbuaoaz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guexdwupq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqwezjrpw.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdxbsfyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelpijrro.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcbajpcw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlygdkok.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadyxgvg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjhrdntv.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdsfykmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzurgqfp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxqppuau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrweqzhj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grecmoakt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gehdvosnr.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gabbgjgga.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwizsyesh.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdzouid.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gshfljyno.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gipopggkz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grnxhvwgi.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgkvnbuf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gylwkgsdv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsxbbujj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gogcnypqj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gofysbucu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbankgpgq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqdowpsw.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gffgskhwz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcxjszvv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvmzdlke.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxlcmsbz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpziuwrz.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqocvhgjc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsiecspq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/glcsfeeiw.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmrfybcw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapchwemy.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gnyjgnydb.sHtML


<!-- 参考信息 -->